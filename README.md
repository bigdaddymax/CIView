CIView
======

View class for Code Igniter to enable flexible layouts usage.

###Usage

- Simply put the View.php file into libraries/ directory of your project
- add <strong>$this->load->library('View');</strong> in your Controller's constructor
- Create <strong>layout.php</strong> file in your views/ directory. This file must to contain $content variable - this is where your content will be inserted
- Use $this->view->render('template_name', $data) instead of $this->load->view('template_name', $data) and your template_name will be inserted into layout automatically.
- If for some reason you don't need a layout to be rendered just call $this->view->enable_layout(FALSE);
- Also you can stack partial templates to construct final page by subsequent calls of $this->view->add_partial('template1'); and then simple $this->view->render(); without arguments
- Basically, that's it

