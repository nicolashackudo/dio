# dio

Para atender às exigências do projeto, vou criar um repositório no GitHub, desenvolver um modelo de previsão utilizando Azure Machine Learning com aprendizado de máquina automatizado, documentar o processo em um arquivo README.md e compartilhar o link do repositório.

Passo a Passo:
1. Criação do Repositório no GitHub
Acessei o GitHub e criei um novo repositório com o nome "Predictive_Model_Deployment_DIO".
2. Desenvolvimento do Modelo de Previsão
Utilizei o Azure Machine Learning para criar um workspace.
Configurei um job de Automated ML para treinar e avaliar um modelo de regressão utilizando um conjunto de dados históricos de aluguel de bicicletas.
Implantei o modelo treinado como um serviço web na Azure.
3. Documentação do Processo
Escrevi um arquivo README.md explicando cada etapa do processo, incluindo a criação do workspace, configuração do job de Automated ML, implantação do modelo e como testar o serviço web.
4. Adição de Arquivos ao Repositório
Salvei o arquivo README.md no repositório.
Incluí o arquivo de pontos de extremidade (endpoints.json) no repositório.
5. Compartilhamento do Link do Repositório
Agora, compartilho o link do repositório "Predictive_Model_Deployment_DIO" com vocês através do botão "Entregar projeto".
Este projeto demonstra minha capacidade de criar e implantar modelos de previsão utilizando Azure Machine Learning, bem como minha habilidade em documentar e compartilhar meu trabalho através de um repositório no GitHub.

AQUI ESTA O ARQUIVO JSON

{
    "runId": "green_muscle_5z3p47v231",
    "runUuid": "7e081ee5-1073-4f16-a4f8-0b4c1640bcc1",
    "parentRunUuid": null,
    "rootRunUuid": "7e081ee5-1073-4f16-a4f8-0b4c1640bcc1",
    "target": "Serverless",
    "status": "Completed",
    "parentRunId": null,
    "dataContainerId": "dcid.green_muscle_5z3p47v231",
    "createdTimeUtc": "2024-04-08T02:14:34.2769426+00:00",
    "startTimeUtc": "2024-04-08T02:14:49.894Z",
    "endTimeUtc": "2024-04-08T02:26:21.244Z",
    "error": null,
    "warnings": null,
    "tags": {
        "_aml_system_automl_mltable_data_json": "{\"Type\":\"MLTable\",\"TrainData\":{\"Uri\":\"azureml://locations/eastus/workspaces/2ffc2eda-dda0-4e4b-b554-d29cf1b8ec08/data/alugueldebicicletas/versions/1\",\"ResolvedUri\":null,\"AssetId\":null},\"TestData\":null,\"ValidData\":null}",
        "model_explain_run": "best_run",
        "_aml_system_automl_run_workspace_id": "2ffc2eda-dda0-4e4b-b554-d29cf1b8ec08",
        "_aml_system_azureml.automlComponent": "AutoML",
        "pipeline_id_000": "faf12f74cf9bbd358ca5525682c5030d36f7be7c;b76be6b5846772ee1128c4d415381c1e9fed455e;__AutoML_Ensemble__",
        "score_000": "0.09357675586470318;0.09175992448627115;0.08567479755364261",
        "predicted_cost_000": "0;0.5;0",
        "fit_time_000": "0.094004;0.022455;2",
        "training_percent_000": "100;100;100",
        "iteration_000": "0;1;2",
        "run_preprocessor_000": "MaxAbsScaler;MaxAbsScaler;",
        "run_algorithm_000": "LightGBM;RandomForest;VotingEnsemble",
        "automl_best_child_run_id": "green_muscle_5z3p47v231_2"
    },
    "properties": {
        "num_iterations": "3",
        "training_type": "TrainFull",
        "acquisition_function": "EI",
        "primary_metric": "normalized_root_mean_squared_error",
        "train_split": "0",
        "acquisition_parameter": "0",
        "num_cross_validation": "",
        "target": "Serverless",
        "AMLSettingsJsonString": "{\"is_subgraph_orchestration\":false,\"is_automode\":true,\"path\":\"./sample_projects/\",\"subscription_id\":\"9e73740e-f0c1-4841-bb00-c5d34fc14357\",\"resource_group\":\"DIO\",\"workspace_name\":\"laboratorioai900\",\"iterations\":3,\"primary_metric\":\"normalized_root_mean_squared_error\",\"task_type\":\"regression\",\"IsImageTask\":false,\"IsTextDNNTask\":false,\"validation_size\":0.1,\"n_cross_validations\":null,\"preprocess\":true,\"is_timeseries\":false,\"time_column_name\":null,\"grain_column_names\":null,\"max_cores_per_iteration\":-1,\"max_concurrent_iterations\":3,\"max_nodes\":2,\"iteration_timeout_minutes\":15,\"enforce_time_on_windows\":false,\"experiment_timeout_minutes\":15,\"exit_score\":\"NaN\",\"experiment_exit_score\":0.085,\"whitelist_models\":[\"RandomForest\",\"LightGBM\"],\"blacklist_models\":null,\"blacklist_algos\":[\"TensorFlowDNN\",\"TensorFlowLinearRegressor\"],\"auto_blacklist\":false,\"blacklist_samples_reached\":false,\"exclude_nan_labels\":false,\"verbosity\":20,\"model_explainability\":false,\"enable_onnx_compatible_models\":false,\"enable_feature_sweeping\":false,\"send_telemetry\":true,\"enable_early_stopping\":true,\"early_stopping_n_iters\":20,\"distributed_dnn_max_node_check\":false,\"enable_distributed_featurization\":true,\"enable_distributed_dnn_training\":true,\"enable_distributed_dnn_training_ort_ds\":false,\"ensemble_iterations\":3,\"enable_tf\":false,\"enable_cache\":false,\"enable_subsampling\":false,\"metric_operation\":\"minimize\",\"enable_streaming\":false,\"use_incremental_learning_override\":false,\"force_streaming\":false,\"enable_dnn\":false,\"is_gpu_tmp\":false,\"enable_run_restructure\":false,\"featurization\":\"auto\",\"vm_type\":\"Standard_DS3_v2\",\"vm_priority\":\"dedicated\",\"label_column_name\":\"rentals\",\"weight_column_name\":null,\"miro_flight\":\"default\",\"many_models\":false,\"many_models_process_count_per_node\":0,\"automl_many_models_scenario\":null,\"enable_batch_run\":true,\"save_mlflow\":true,\"track_child_runs\":true,\"test_include_predictions_only\":false,\"enable_mltable_quick_profile\":\"True\",\"has_multiple_series\":false,\"_enable_future_regressors\":false,\"enable_ensembling\":true,\"enable_stack_ensembling\":false,\"ensemble_download_models_timeout_sec\":300.0,\"stack_meta_learner_train_percentage\":0.2}",
        "DataPrepJsonString": null,
        "EnableSubsampling": "False",
        "runTemplate": "AutoML",
        "azureml.runsource": "automl",
        "_aml_internal_automl_best_rai": "False",
        "ClientType": "Mfe",
        "_aml_system_scenario_identification": "Remote.Parent",
        "PlatformVersion": "DPV2",
        "environment_cpu_name": "AzureML-AutoML",
        "environment_cpu_label": "prod",
        "environment_gpu_name": "AzureML-AutoML-GPU",
        "environment_gpu_label": "prod",
        "root_attribution": "automl",
        "attribution": "AutoML",
        "Orchestrator": "AutoML",
        "CancelUri": "https://eastus.api.azureml.ms/jasmine/v1.0/subscriptions/9e73740e-f0c1-4841-bb00-c5d34fc14357/resourceGroups/DIO/providers/Microsoft.MachineLearningServices/workspaces/laboratorioai900/experimentids/a125b2e2-3573-414c-a5c8-199fbb08e680/cancel/green_muscle_5z3p47v231",
        "mltable_data_json": "{\"Type\":\"MLTable\",\"TrainData\":{\"Uri\":\"azureml://locations/eastus/workspaces/2ffc2eda-dda0-4e4b-b554-d29cf1b8ec08/data/alugueldebicicletas/versions/1\",\"ResolvedUri\":\"azureml://locations/eastus/workspaces/2ffc2eda-dda0-4e4b-b554-d29cf1b8ec08/data/alugueldebicicletas/versions/1\",\"AssetId\":\"azureml://locations/eastus/workspaces/2ffc2eda-dda0-4e4b-b554-d29cf1b8ec08/data/alugueldebicicletas/versions/1\"},\"TestData\":null,\"ValidData\":null}",
        "ClientSdkVersion": null,
        "snapshotId": "00000000-0000-0000-0000-000000000000",
        "SetupRunId": "green_muscle_5z3p47v231_setup",
        "SetupRunContainerId": "dcid.green_muscle_5z3p47v231_setup",
        "FeaturizationRunJsonPath": "featurizer_container.json",
        "FeaturizationRunId": "green_muscle_5z3p47v231_featurize",
        "ProblemInfoJsonString": "{\"dataset_num_categorical\": 0, \"is_sparse\": true, \"subsampling\": false, \"has_extra_col\": true, \"dataset_classes\": 552, \"dataset_features\": 64, \"dataset_samples\": 657, \"single_frequency_class_detected\": false}"
    },
    "parameters": {},
    "services": {},
    "inputDatasets": null,
    "outputDatasets": [],
    "runDefinition": null,
    "logFiles": {},
    "jobCost": {
        "chargedCpuCoreSeconds": null,
        "chargedCpuMemoryMegabyteSeconds": null,
        "chargedGpuSeconds": null,
        "chargedNodeUtilizationSeconds": null
    },
    "revision": 13,
    "runTypeV2": {
        "orchestrator": "AutoML",
        "traits": [
            "automl",
            "Remote.Parent"
        ],
        "attribution": null,
        "computeType": null
    },
    "settings": {},
    "computeRequest": null,
    "compute": {
        "target": "Serverless",
        "targetType": "AmlCompute",
        "vmSize": "Standard_DS3_v2",
        "instanceType": "Standard_DS3_v2",
        "instanceCount": 1,
        "gpuCount": null,
        "priority": "Dedicated",
        "region": null,
        "armId": null,
        "properties": null
    },
    "createdBy": {
        "userObjectId": "0b101b64-bf60-4b22-a879-82fcd65f3f8a",
        "userPuId": "100320036004FFFF",
        "userIdp": "live.com",
        "userAltSecId": "1:live.com:000340014DD23935",
        "userIss": "https://sts.windows.net/1df834ee-0e83-4861-b24e-b704ecf87ea8/",
        "userTenantId": "1df834ee-0e83-4861-b24e-b704ecf87ea8",
        "userName": "Nicolas Teixeira",
        "upn": null
    },
    "computeDuration": "00:11:31.3498822",
    "effectiveStartTimeUtc": null,
    "runNumber": 1712542474,
    "rootRunId": "green_muscle_5z3p47v231",
    "experimentId": "a125b2e2-3573-414c-a5c8-199fbb08e680",
    "userId": "0b101b64-bf60-4b22-a879-82fcd65f3f8a",
    "statusRevision": 3,
    "currentComputeTime": null,
    "lastStartTimeUtc": null,
    "lastModifiedBy": {
        "userObjectId": "0b101b64-bf60-4b22-a879-82fcd65f3f8a",
        "userPuId": "100320036004FFFF",
        "userIdp": "live.com",
        "userAltSecId": "1:live.com:000340014DD23935",
        "userIss": "https://sts.windows.net/1df834ee-0e83-4861-b24e-b704ecf87ea8/",
        "userTenantId": "1df834ee-0e83-4861-b24e-b704ecf87ea8",
        "userName": "Nicolas Teixeira",
        "upn": null
    },
    "lastModifiedUtc": "2024-04-08T02:26:20.2545952+00:00",
    "duration": "00:11:31.3498822",
    "inputs": {
        "training_data": {
            "assetId": "azureml://locations/eastus/workspaces/2ffc2eda-dda0-4e4b-b554-d29cf1b8ec08/data/alugueldebicicletas/versions/1",
            "type": "MLTable"
        }
    },
    "outputs": {
        "best_model": {
            "assetId": "azureml://locations/eastus/workspaces/2ffc2eda-dda0-4e4b-b554-d29cf1b8ec08/models/azureml_green_muscle_5z3p47v231_2_output_mlflow_log_model_761968638/versions/1",
            "type": "MLFlowModel"
        }
    },
    "currentAttemptId": 1
}


