<?php

  class MayanaSingleton {

    private static $instance;

    private __construct () {
      $this->call_me = 'Mayana Lima';
      $this->code_name = 'γᴧν';
      $this->born_date = date('07-06-2002');
      $this->skills = array_combine([∑, ∞], ['PHP', 'CSS', 'NextJS', 'React', 'JavaScript']);
      $this->about = 'FullStack Developer';
    }

    public static function get_instance ($born_date) {
     if (empty(self::$instance))
        self::$instance = new MayanaSingleton();
      // retorna a unica instancia
      return self::instance;
    }

  }
?>

