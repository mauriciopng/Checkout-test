<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-QWTKZyjpPEjISv5WaRU9OFeRpok6YctnYmDr5pNlyT2bRjXh0JMhjY6hW+ALEwIH" crossorigin="anonymous">
    <title>checkout</title>
</head>
<body>
    <div class="container">
        <main>
          <div class="py-5 text-center">
            <h2>Pagamento </h2>
            <p class="lead">A um passo para finalizar sua compra ! </p>
          </div>
      
          <div class="row g-5">
            <div class="col-md-5 col-lg-4 order-md-last">
              <h4 class="d-flex justify-content-between align-items-center mb-3">
                <span class="text-primary">Seu Carrinho</span>
                <span class="badge bg-primary rounded-pill">3</span>
              </h4>
              <ul class="list-group mb-3">
                <li class="list-group-item d-flex justify-content-between lh-sm">
                  <div>
                    <h6 class="my-0">Primeiro Produto</h6>
                    <small class="text-body-secondary">Descrição do produto</small>
                  </div>
                  <span class="text-body-secondary">R$12</span>
                </li>
                <li class="list-group-item d-flex justify-content-between lh-sm">
                  <div>
                    <h6 class="my-0">Segundo Produto</h6>
                    <small class="text-body-secondary">Descrição do produto</small>
                  </div>
                  <span class="text-body-secondary">R$8</span>
                </li>
                <li class="list-group-item d-flex justify-content-between lh-sm">
                  <div>
                    <h6 class="my-0">Terceiro Produto</h6>
                    <small class="text-body-secondary">Descrição do produto</small>
                  </div>
                  <span class="text-body-secondary">R$5</span>
                </li>
                <li class="list-group-item d-flex justify-content-between bg-body-tertiary">
                  <div class="text-success">
                    <h6 class="my-0">Código promocional</h6>
                    <small>CÓDIGOEXEMPLO</small>
                  </div>
                  <span class="text-success">−$5</span>
                </li>
                <li class="list-group-item d-flex justify-content-between">
                  <span>Total (R$)</span>
                  <strong>R$20</strong>
                </li>
              </ul>
      
              <form class="card p-2">
                <div class="input-group">
                  <input type="text" class="form-control" placeholder="Código promocional">
                  <button type="submit" class="btn btn-secondary">Confimar</button>
                </div>
              </form>
            </div>
            <div class="col-md-7 col-lg-8">
              <h4 class="mb-3">Endereço de Pagamento</h4>
              <form class="needs-validation" novalidate>
                <div class="row g-3">
                  <div class="col-sm-6">
                    <label for="firstName" class="form-label">Primeiro Nome</label>
                    <input type="text" class="form-control" id="firstName" placeholder="" value="" required>
                    <div class="invalid-feedback">
                        Necessário Validar seu primeiro nome
                    </div>
                  </div>
      
                  <div class="col-sm-6">
                    <label for="lastName" class="form-label">Ultimo nome</label>
                    <input type="text" class="form-control" id="lastName" placeholder="" value="" required>
                    <div class="invalid-feedback">
                      Necessário Validar seu último nome
                    </div>
                  </div>
      
                  <div class="col-12">
                    <label for="username" class="form-label">E-mail</label>
                    <div class="input-group has-validation">
                      <span class="input-group-text">@</span>
                      <input type="text" class="form-control" id="username" placeholder="nome de usuário" required>
                    <div class="invalid-feedback">
                       Necessário seu endereço E-mail.
                      </div>
                    </div>
                  </div>
      
                  <div class="col-12">
                    <label for="email" class="form-label">Email <span class="text-body-secondary">(Optional)</span></label>
                    <input type="email" class="form-control" id="email" placeholder="seu@exemplo.com">
                    <div class="invalid-feedback">
                      Por favor, preencha com o seu E-mail para mais informações
                    </div>
                  </div>
      
                  <div class="col-12">
                    <label for="address" class="form-label">Endereço</label>
                    <input type="text" class="form-control" id="address" placeholder="Rua num1234..." required>
                    <div class="invalid-feedback">
                     Por favor, preencha com o seu endereço.
                    </div>
                  </div>
      
                  <div class="col-12">
                    <label for="address2" class="form-label">Endereço 2 <span class="text-body-secondary">(Optional)</span></label>
                    <input type="text" class="form-control" id="address2" placeholder="Casa ou apartamento">
                  </div>
      
                  <div class="col-md-5">
                    <label for="country" class="form-label">Pais</label>
                    <select class="form-select" id="country" required>
                      <option value="">Escolha...</option>
                      <option>Brasil</option>
                    </select>
                    <div class="invalid-feedback">
                     Por favor, preencha com um pais válido
                    </div>
                  </div>
      
                  <div class="col-md-4">
                    <label for="state" class="form-label">Estado</label>
                    <select class="form-select" id="state" required>
                      <option value="">Escolha...</option>
                      <option>Rio de janeiro</option>
                    </select>
                    <div class="invalid-feedback">
                      Por favor, preencha com um estado válido
                    </div>
                  </div>
      
                  <div class="col-md-3">
                    <label for="zip" class="form-label">DDD</label>
                    <input type="text" class="form-control" id="zip" placeholder="" required>
                    <div class="invalid-feedback">
                      DDD obrigatório.
                    </div>
                  </div>
                </div>
      
                <hr class="my-4">
      
                <div class="form-check">
                  <input type="checkbox" class="form-check-input" id="same-address">
                  <label class="form-check-label" for="same-address">Endereço de entrega é o mesmo endereço de cobrança</label>
                </div>
      
                <div class="form-check">
                  <input type="checkbox" class="form-check-input" id="save-info">
                  <label class="form-check-label" for="save-info">Salvar as informações para as próxximas vezes.</label>
                </div>
      
                <hr class="my-4">
      
                <h4 class="mb-3">Pagamento</h4>
      
                <div class="my-3">
                  <div class="form-check">
                    <input id="credit" name="paymentMethod" type="radio" class="form-check-input" checked required>
                    <label class="form-check-label" for="credit">Cartão de Crédito</label>
                  </div>
                  <div class="form-check">
                    <input id="debit" name="paymentMethod" type="radio" class="form-check-input" required>
                    <label class="form-check-label" for="debit">Cartão de Débito</label>
                  </div>
                  <div class="form-check">
                    <input id="paypal" name="paymentMethod" type="radio" class="form-check-input" required>
                    <label class="form-check-label" for="paypal">Pix</label>
                  </div>
                </div>
      
                <div class="row gy-3">
                  <div class="col-md-6">
                    <label for="cc-name" class="form-label">Nome no Cartão</label>
                    <input type="text" class="form-control" id="cc-name" placeholder="" required>
                    <small class="text-body-secondary">Nome completo como presente no Cartão      
                    </small>
                    <div class="invalid-feedback">
                     Nome no cartão necessário.
                    </div>
                  </div>
      
                  <div class="col-md-6">
                    <label for="cc-number" class="form-label">Número do Cartão de crédito</label>
                    <input type="text" class="form-control" id="cc-number" placeholder="" required>
                    <div class="invalid-feedback">
                        Número do Cartão de crédito necessário
                    </div>
                  </div>
      
                  <div class="col-md-3">
                    <label for="cc-expiration" class="form-label">Validade</label>
                    <input type="text" class="form-control" id="cc-expiration" placeholder="" required>
                    <div class="invalid-feedback">
                      Data de validade necessário
                    </div>
                  </div>
      
                  <div class="col-md-3">
                    <label for="cc-cvv" class="form-label">CVV</label>
                    <input type="text" class="form-control" id="cc-cvv" placeholder="" required>
                    <div class="invalid-feedback">
                      Código de segurança necessário
                    </div>
                  </div>
                </div>
      
                <hr class="my-4">
      
                <button class="w-100 btn btn-primary btn-lg" type="submit">Continuar checkout</button>
              </form>
            </div>
          </div>
        </main>

        <footer>
            <p class="mb-1">&copy; –2024 Maurício</p>
            <ul class="list-inline">
              <li class="list-inline-item"><a href="#">Privacy</a></li>
              <li class="list-inline-item"><a href="#">Terms</a></li>
              <li class="list-inline-item"><a href="#">Support</a></li>
            </ul>
          </footer>

        </footer>
</body>
</html>
