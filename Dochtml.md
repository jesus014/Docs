<div class="container">
  <div class="row">

       <div class="col-md-6 col-sm-6">
            <img src="assets/images/appointment-image.jpg" class="img-responsive" alt="">
       </div>

       <div class="col-md-6 col-sm-6">
            <!-- CONTACT FORM HERE -->
            <form (ngSubmit)="onSubmit(contactForm)"  #contactForm="ngForm"  id="appointment-form" role="form" method="post" action="#">

                 <!-- SECTION TITLE -->
                 <div class="section-title wow fadeInUp" data-wow-delay="0.4s">
                      <h2>¡Contactanos!</h2>
                 </div>

                 <div class="wow fadeInUp" data-wow-delay="0.8s">
                      <div class="col-md-6 col-sm-6">
                           <label for="name">Nombre</label>
                           <input type="text" class="form-control" id="name" name="name" placeholder="Nombre Completo"  ngModel #name="ngModel" required>
                      </div>

                      <div class="col-md-6 col-sm-6">
                           <label for="email">Email</label>
                           <input type="email" class="form-control" id="email" name="email" placeholder="example@hotmail.com"  ngModel required #email="ngModel">
                      </div>

                      <div class="col-md-6 col-sm-6">
                           <label for="date"> Fecha</label>
                           <input type="date" name="date" value=""   ngModel  #date="ngModel"  class="form-control"  required>
                      </div>

                      <div class="col-md-6 col-sm-6">
                           <label for="select">Selecione el Departamento</label>
                           <select class="form-control" name="tipo" ngModel  #tipo="ngModel" >
                                <option>General Health</option>
                                <option>Cardiology</option>
                                <option>Dental</option>
                                <option>Medical Research</option>
                           </select>
                      </div>

                      <div class="col-md-12 col-sm-12">
                           <label for="telephone">Numero de telefono</label>
                           <input type="tel" class="form-control" id="phone" name="phone" ngModel  #phone="ngModel" placeholder="Phone" required >
                           <label for="Message">Mensaje </label>
                           <textarea class="form-control" rows="5" id="messages" name="messages" placeholder="Escriba un mensaje" ngModel  #messages="ngModel"></textarea>
                           <button type="submit" class="form-control" id="cf-submit" name="submit">Enviar Duda</button>
                      </div>
                 </div>
           </form>
       </div>
  </div>
</div>
