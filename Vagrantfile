
Vagrant.configure("2") do |config|
  
  config.vm.box = "ubuntu/xenial64"
  config.vm.hostname = "jorge-fresno-menendez"


   config.vm.provision "shell", inline: <<-SHELL
  echo "-- Insertar datos de ejemplo en la tabla 'libros'" > /home/vagrant/datos_libros.sql
  echo "INSERT INTO gestion_libreria.libros (titulo, autor, anio_publicacion, genero, precio) VALUES">> /home/vagrant/datos_libros.sql
  echo "('Cien Años de Soledad', 'Gabriel García Márquez', 1605, 'Novela', 12.99),">> /home/vagrant/datos_libros.sql
  echo "('Cien Años de Soledad', 'Gabriel García Márquez', 1605, 'Novela', 12.99),">> /home/vagrant/datos_libros.sql
  echo "('Cien Años de Soledad', 'Gabriel García Márquez', 1605, 'Novela', 12.99)">> /home/vagrant/datos_libros.sql
   SHELL
end
