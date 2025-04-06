<h1>Pesquisa e Análise com Azure AI e Storage</h1>

<h2>Ferramentas para Pesquisa</h2>
<p>
  Para reconhecimento e análise de arquivos (mídia ou texto), utilizamos o <strong>Blob Storage</strong>, que permite integração via API REST. Para armazenar grandes volumes de dados, utilizamos o <strong>Data Lake Storage</strong>, podendo integrar com <strong>tabelas de bancos de dados relacionais</strong>.
</p>

<h2>Início</h2>
<p>
  Em cenários com alto volume de dados, utilizamos <strong>índices</strong> para alimentar e estruturar a base de dados. O <strong>formato JSON</strong> é ideal para pesquisas, por sua compatibilidade e facilidade de exploração.
</p>

<h2>Pesquisa de Campo</h2>
<p>
  Quanto mais dados coletamos, mais precisos serão os resultados. Um exemplo prático: uma loja pode descobrir informações sobre:
</p>
<ul>
  <li>Comércios ao redor (logística e concorrência);</li>
  <li>Público-alvo local;</li>
  <li>Horários de maior movimento;</li>
  <li>Tendências e poder aquisitivo de clientes.</li>
</ul>

<h2>Etapas para uma Pesquisa Eficaz</h2>
<p>No laboratório, seguimos três passos principais:</p>
<ol>
  <li><strong>Ingestão</strong> dos dados;</li>
  <li><strong>Enriquecimento</strong> com uso de índices;</li>
  <li><strong>Exploração</strong> das informações.</li>
</ol>

<h2>Trabalhando com os Dados</h2>
<p>
  Utilizamos o <strong>Azure AI Search</strong> para buscar dados sobre a reputação de uma loja ou empresa. Podemos extrair essas informações via aplicativo e alimentar a IA, trabalhando com índices para melhorar a pesquisa.
</p>

<h2>Passo a Passo no Azure</h2>

<h3>1. Criar o Azure AI Search</h3>
<ul>
  <li>Acesse o portal Azure;</li>
  <li>Pesquise por <strong>Azure AI Search</strong>;</li>
  <li>Clique em <strong>Create</strong> e preencha: <em>Resource Group</em>, <em>Service Name</em> e <em>Location</em>;</li>
  <li>Escolha o plano de serviço;</li>
  <li>Finalize com <strong>Review + Create</strong>.</li>
</ul>

<h3>2. Criar o Azure AI Services</h3>
<ul>
  <li>Clique em <strong>Create Resource</strong>;</li>
  <li>Escolha <strong>Azure AI Services</strong>;</li>
  <li>Repita os mesmos passos anteriores de configuração.</li>
</ul>

<h3>3. Criar o Storage Account</h3>
<ul>
  <li>Acesse <strong>Create Resource</strong>;</li>
  <li>Escolha <strong>Storage Account</strong>;</li>
  <li>Preencha os campos em <strong>Basics</strong>;</li>
  <li>No menu lateral, vá em <strong>Settings > Configuration</strong>;</li>
  <li>Ative a opção <strong>Allow storage account key access</strong> e clique em <strong>Save</strong>.</li>
</ul>

<h3>4. Criar e Alimentar Containers</h3>
<ul>
  <li>Vá no menu lateral do Storage Account e clique em <strong>Containers</strong>;</li>
  <li>Crie um novo container com um nome personalizado;</li>
  <li>Dentro do container, use a opção <strong>Upload</strong> para enviar arquivos (ex: .docx).</li>
</ul>

<h2>Exploração dos Dados</h2>
<p>
  Agora, com todos os serviços configurados, vamos iniciar a exploração:
</p>
<ul>
  <li>Acesse o <strong>Azure AI Search</strong>;</li>
  <li>Clique em <strong>Import Data</strong> e selecione o Storage Account com os arquivos enviados;</li>
  <li>Vá em <strong>Search Explorer</strong> e utilize <strong>queries</strong> para filtrar dados por localização, qualificação de serviços, etc.</li>
</ul>
<p>
  Essas informações podem ser utilizadas por aplicativos para gerar insights e funcionalidades inteligentes baseadas nos dados.
</p>
