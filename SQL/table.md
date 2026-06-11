USE test_db;

CREATE TABLE IF NOT EXISTS files (
    id INT AUTO_INCREMENT PRIMARY KEY,
    file_name VARCHAR(255) NOT NULL,
    category VARCHAR(100),
    created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP
);

INSERT INTO files (file_name, category) VALUES 
('network_parameter_sheet.xlsx', 'Network'),
('cisco_catalyst_config.txt', 'Network'),
('ubuntu_setup_guide.md', 'OS'),
('apache_vhost_backup.conf', 'Server'),
('mysql_secure_install_log.txt', 'Security'),
('portfolio_architecture.pdf', 'Document');

SELECT * FROM files;
