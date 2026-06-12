# Curso de Machine Learning e Visão Computacional

Repositório de estudos para organizar as aulas, atividades práticas e desafios da trilha de Machine Learning com foco em Visão Computacional.

O curso começa com fundamentos de programação científica em Python, avança para processamento de imagens e aprendizagem de máquina, passa por redes neurais convolucionais, modelos pré-treinados, modelos gerativos e aplicações reais, e termina com tópicos de MLOps.

## Objetivo

Manter em um único lugar:

- notebooks originais das aulas;
- imagens, modelos e arquivos auxiliares usados nas práticas;
- scripts próprios de resolução e experimentação;
- anotações em Markdown por módulo, aula e desafio;
- registro versionado da evolução do curso.

## Estrutura

```text
.
├── modulo_01/
├── modulo_02/
├── modulo_03/
├── modulo_04/
├── modulo_05/
├── modulo_06/
├── desafios/
├── requirements.txt
└── README.md
```

Cada módulo reúne aulas práticas em notebooks Jupyter. A pasta `desafios/` reúne atividades maiores que combinam os conceitos aprendidos ao longo da trilha.

## Módulos

### Módulo 1: Fundamentos de programação para visão computacional

Introduz a base técnica para manipular imagens com Python.

Conteúdos principais:

- visão computacional;
- arrays com NumPy;
- visualização de imagens;
- OpenCV;
- operações básicas em imagens;
- imagens digitais;
- filtros espaciais e convoluções;
- processamento de vídeo.

Aulas disponíveis no repositório:

- `aula_02`: manipulação de arrays com NumPy;
- `aula_03`: visualização de imagens;
- `aula_04`: introdução ao OpenCV;
- `aula_05`: operações básicas em imagens;
- `aula_07`: filtros espaciais e convoluções.

### Módulo 2: Aprendizagem de máquina aplicada à visão

Conecta processamento de imagem com técnicas clássicas e modernas de Machine Learning.

Conteúdos principais:

- detecção e extração de características;
- correspondência de características;
- classificadores supervisionados;
- divisão de dados;
- métricas de desempenho;
- visualização de resultados;
- redes neurais;
- visão com aprendizado profundo;
- CNNs;
- modelos pré-treinados.

Aulas disponíveis no repositório:

- `aula_02`: detecção e extração de características;
- `aula_03`: correspondência de características;
- `aula_10`: modelos pré-treinados.

### Módulo 3: Redes neurais convolucionais

Aprofunda o uso de redes neurais modernas para tarefas visuais.

Conteúdos principais:

- revisão de aprendizado profundo;
- topologias contemporâneas;
- transfer learning;
- refinamento com redes pré-treinadas;
- classificação de imagens;
- detecção de objetos;
- segmentação semântica.

Aulas disponíveis no repositório:

- `aula_03`: transfer learning e refinamento;
- `aula_05`: detecção de objetos;
- `aula_06`: segmentação semântica.

### Módulo 4: Modelos gerativos

Apresenta técnicas modernas de geração e uso multimodal.

Conteúdos principais:

- autoencoders variacionais;
- GANs;
- modelos de difusão;
- GenAI para data augmentation;
- modelos multimodais.

Aulas disponíveis no repositório:

- `aula_02`: GANs;
- `aula_05`: fundamentos de modelos multimodais.

### Módulo 5: Projetos reais de visão computacional

Aplica modelos e pipelines em cenários mais próximos de problemas reais.

Conteúdos principais:

- inspeção visual em manufatura;
- reconhecimento de texto;
- identificação de elementos visuais em UI;
- sistema de vigilância;
- segmentação de falhas em tecidos;
- detecção de faixas para veículos autônomos.

Aulas disponíveis no repositório:

- `aula_01`: inspeção visual de itens em esteira;
- `aula_02`: reconhecimento de texto;
- `aula_03`: identificação de elementos visuais em UI;
- `aula_04`: sistema de vigilância;
- `aula_05`: segmentação de falhas em tecidos;
- `aula_06`: detecção de faixas para veículos autônomos.

### Módulo 6: MLOps

Introduz práticas de acompanhamento, organização e monitoramento de experimentos.

Conteúdos principais:

- conceitos de MLOps;
- refinamento de hiperparâmetros;
- monitoramento de experimentos.

Aula disponível no repositório:

- `aula_03`: sistemas de monitoramento de experimentos.

## Desafios

Os desafios funcionam como projetos práticos de consolidação.

- `desafio_01`: aplicação de desfoque no fundo de uma imagem com pessoa, simulando efeito de videochamada.
- `desafio_02`: reconhecimento facial, semelhante a sistemas simples de controle de acesso.
- `desafio_03`: rastreamento de objetos em imagens ou vídeos.
- `desafio_04`: reconhecimento de poses, útil em aplicações como análise esportiva.

## Pré-requisitos

Para aproveitar bem o curso, é recomendado ter:

- noções básicas de Python;
- familiaridade mínima com terminal Linux/WSL;
- Git e GitHub para versionamento;
- VS Code com extensões Python e Jupyter;
- entendimento básico de matrizes, vetores e funções;
- disposição para executar e modificar notebooks manualmente.

Conhecimentos de Machine Learning ajudam, mas o curso também constrói boa parte dessa base durante as práticas.

## Ambiente Necessário

Ferramentas recomendadas:

- Python 3.10 ou superior;
- ambiente virtual Python (`venv`);
- Jupyter Notebook ou VS Code com suporte a notebooks;
- Git;
- conexão com a internet para baixar bibliotecas, datasets e modelos;
- GPU opcional para treinos mais pesados com PyTorch/YOLO.

O ambiente local deste repositório usa uma pasta `.venv`, que não deve ser enviada ao GitHub.

## Configuração Inicial

Crie e ative o ambiente virtual:

```bash
python3 -m venv .venv
source .venv/bin/activate
```

Atualize o `pip`:

```bash
python -m pip install --upgrade pip
```

Instale o conjunto básico de dependências:

```bash
python -m pip install -r requirements.txt
```

Abra o Jupyter:

```bash
jupyter notebook
```

Ou use os notebooks diretamente pelo VS Code, selecionando o kernel da `.venv`.

## Dependências

O arquivo `requirements.txt` contém o kit básico usado nos primeiros módulos:

- NumPy;
- Pandas;
- Matplotlib;
- Scikit-learn;
- Seaborn;
- Jupyter;
- Notebook;
- OpenCV.

Algumas aulas avançadas instalam dependências extras conforme necessário. Pelos notebooks do curso, aparecem principalmente:

```bash
python -m pip install torch torchvision
python -m pip install ultralytics
python -m pip install easyocr
python -m pip install imutils tqdm ipywidgets
python -m pip install datasets huggingface_hub
python -m pip install tensorboard
python -m pip install torchcodec ffmpeg-python av
python -m pip install git+https://github.com/openai/CLIP.git
```

Nem todas precisam ser instaladas de uma vez. A melhor estratégia é instalar conforme a aula pedir.

## Fluxo de Estudo

Para cada aula:

1. Abra o notebook original.
2. Leia as células de Markdown antes de executar código.
3. Execute célula por célula.
4. Verifique os caminhos de imagens, datasets e modelos.
5. Reproduza os exemplos em um script próprio quando fizer sentido.
6. Registre dúvidas e aprendizados no `README.md` da aula ou do módulo.
7. Faça commit das alterações relevantes.

Exemplo de rotina com Git:

```bash
git status
git add .
git commit -m "adiciona anotacoes da aula"
git push
```

## Cuidados

- Não versionar `.venv/`, caches ou checkpoints de notebook.
- Conferir caminhos relativos antes de executar notebooks copiados de outro diretório.
- Evitar subir datasets muito grandes se não forem necessários.
- Manter modelos pesados apenas quando forem parte essencial da atividade.
- Preferir nomes de pastas sem espaços e sem acentos para facilitar o uso no terminal.

## Observações Sobre Notebooks

Arquivos `.ipynb` são notebooks Jupyter. Para abri-los corretamente no VS Code, instale e habilite as extensões:

- Python;
- Jupyter.

Se o VS Code abrir o notebook como texto JSON ou mostrar erro de `jupyter-notebook`, habilite a extensão Jupyter no ambiente local ou WSL.

## Status

Este repositório está em construção conforme os materiais do curso forem sendo organizados e estudados.
