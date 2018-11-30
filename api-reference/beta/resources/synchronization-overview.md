---
title: Обзор синхронизации API Azure AD
description: ') позволяет автоматизировать создания, обслуживания и удаления удостоверений в облако (программное обеспечение как службы или SaaS) приложениями, такими как общего банка данных, Salesforce, ServiceNow и многое другое. API синхронизации можно использовать в Microsoft Graph для управления синхронизацией identity программным путем, включая:'
ms.openlocfilehash: ff3acb00801c9b04b8257345b06100297e11710c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081460"
---
# <a name="azure-ad-synchronization-api-overview"></a>Обзор синхронизации API Azure AD

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Azure (Azure AD) удостоверений синхронизации с Active Directory (также называемая «Подготовка») позволяет автоматизировать создания, обслуживания и удаления удостоверений в облаке (программное обеспечение как службы или SaaS) приложениями, такими как общего банка данных, Salesforce, ServiceNow, и многое другое. API синхронизации можно использовать в Microsoft Graph для управления синхронизацией identity программным путем, включая:

- Создание, запуск и остановка задания синхронизации
- Вносить изменения в схеме синхронизации для задания
- Проверка текущего состояния синхронизации 

Дополнительные сведения о синхронизации в Azure AD см.

* [Автоматизировать пользователя обеспечение и Отмена обеспечения SaaS приложений с помощью Azure Active Directory](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-saas-app-provisioning)
* [Управление для корпоративных приложений в портале Azure при подготовке учетной записи пользователя](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-enterprise-apps-manage-provisioning)

Можно также попробовать API в [Обозревателе график](https://developer.microsoft.com/graph/graph-explorer) в пример клиента или собственного клиента.

## <a name="synchronization-job"></a>Задание синхронизации

Задания синхронизации для выполнения синхронизации периодически выполняется в фоновом режиме, опроса для изменения в один каталог и помещает их в другой каталог. Задание синхронизации всегда специально для конкретного экземпляра приложения клиента. Как часть процесса установки задания синхронизации необходимо предоставить разрешение на чтение и запись в целевом каталоге объекты и настройке задания синхронизации схемы.

Для получения дополнительных сведений см [Задание синхронизации](synchronization-synchronizationjob.md).

## <a name="synchronization-schema"></a>Схема синхронизации

Схема синхронизации определяет объекты, которые будут синхронизированы и как они будут синхронизироваться. Схема синхронизации содержит основные сведения об установке для задания синхронизации. Как правило будет настроить некоторые [атрибут сопоставления](synchronization-attributemapping.md)или добавить [области видимости фильтров](synchronization-filter.md) синхронизировать только объекты, удовлетворяющие определенному условию.

Схема синхронизации включает в себя следующие компоненты:

- Определения каталогов
- Правила синхронизации
- Объект сопоставления

Для получения дополнительных сведений см [синхронизации](synchronization-synchronizationschema.md).

## <a name="synchronization-template"></a>Шаблон синхронизации

Шаблон синхронизации предоставляет параметры предварительно настроенным синхронизации для конкретного приложения. Эти параметры (важнее, [синхронизации схемы](synchronization-synchronizationschema.md)) будет использоваться по умолчанию для любое [Задание синхронизации](synchronization-synchronizationjob.md) , основанный на шаблоне. Шаблоны задаются разработчиком приложения.

Для получения дополнительных сведений см [шаблон синхронизации](synchronization-synchronizationtemplate.md).

## <a name="working-with-the-synchronization-api"></a>Работа с API синхронизации

Работа с синхронизацией API в основном состоит из доступ к ресурсам [synchronizationJob](synchronization-synchronizationjob.md) и [synchronizationSchema](synchronization-synchronizationschema.md) . Чтобы найти [synchronizationJob](synchronization-synchronizationjob.md) ресурса, необходимо знать идентификатор объекта-участника службы, к которой принадлежит задание синхронизации. В приведенных ниже примерах показано, как работать с ресурсами **synchronizationJob** и **synchronizationSchema** .

### <a name="authorization"></a>Authorization

Интерфейс API синхронизации Azure AD для авторизации используется OAuth 2.0. Прежде чем вносить какие-либо запросы API-интерфейса, необходимо получить маркер доступа. Для получения дополнительных сведений см [маркеры доступа Get для вызова Microsoft Graph](https://developer.microsoft.com/graph/docs/concepts/auth_overview). Для доступа к ресурсам синхронизации, приложению Directory.ReadWrite.All разрешения. Для получения дополнительных сведений см [разрешения для каталога](/graph/permissions-reference#directory-permissions).

### <a name="find-the-service-principal-object-by-display-name"></a>Найдите объект участника службы по отображаемому имени

Следующем примере показано, как для объекта-участника службы поиска по отображаемому имени.

**Запрос** 

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/servicePrincipals?$select=id,appId,displayName&$filter=startswith(displayName, 'salesforce')
```

**Отклик**

<!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
{
    "value": [
    {
        "id": "bc0dc311-87df-48ac-91b1-259bd2c3a31c",
        "appId": "f7808c5e-cb57-4e37-8094-406d302c0f8d",
        "displayName": "Salesforce"
    },
    {
        "id": "d813d7d7-0f41-4edc-b284-d0dfaf399d15",
        "appId": "219561ee-1480-4c67-9aa6-63d861fae3ef",
        "displayName": "salesforce 3"
    }
    ]
}
```

### <a name="find-the-service-principal-object-by-app-id"></a>Найдите объект участника службы по Идентификатору приложения

Следующем примере показано, как найти объекта участника-службы с идентификатором приложения.

**Запрос** 
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/servicePrincipals?$select=id,appId,displayName&$filter=AppId eq '219561ee-1480-4c67-9aa6-63d861fae3ef'
```

**Ответа**
<!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
{
    "value": [
        {
            "id": "d813d7d7-0f41-4edc-b284-d0dfaf399d15",
            "appId": "219561ee-1480-4c67-9aa6-63d861fae3ef",
            "displayName": "salesforce 3"
        }
    ]
}
```

### <a name="list-existing-synchronization-jobs"></a>Список существующих заданий синхронизации

Следующем примере показано, как список существующих заданий синхронизации.

**Запрос**
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs
GET https://graph.microsoft.com/beta/servicePrincipals/60443998-8cf7-4e61-b05c-a53b658cb5e1/synchronization/jobs
```

**Ответа**
<!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
{
    "value": [
        {
            "id": "SfSandboxOutDelta.e4bbf44533ea4eabb17027f3a92e92aa",
            "templateId": "SfSandboxOutDelta",
            "schedule": {
                "expiration": null,
                "interval": "PT20M",
                "state": "Active"
            },
            "status": {}
        }
    ]
}
```

### <a name="get-synchronization-job-status"></a>Получить сведения о состоянии задания синхронизации
Следующем примере показано, как получить сведения о состоянии задания синхронизации.

**Запрос**
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}

GET https://graph.microsoft.com/beta/servicePrincipals/60443998-8cf7-4e61-b05c-a53b658cb5e1/synchronization/jobs/SfSandboxOutDelta.e4bbf44533ea4eabb17027f3a92e92aa
```

**Ответа**
<!-- { "blockType": "ignored" } -->
```http
    HTTP/1.1 200 OK
    {
        "id": "SfSandboxOutDelta.e4bbf44533ea4eabb17027f3a92e92aa",
        "templateId": "SfSandboxOutDelta",
        "schedule": {
            "expiration": null,
            "interval": "PT20M",
            "state": "Active"
        },
        "status": {}
    }
```

### <a name="get-synchronization-schema"></a>Получение схемы синхронизации
Следующем примере показано, как получить схему синхронизации.

**Запрос**
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
```

**Ответа**
<!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
{
    "directories": [],
    "synchronizationRules": []
}
```
## <a name="see-also"></a>См. также

* [Настройка синхронизации с расширением атрибутов каталога](../resources/synchronization-configure-with-directory-extension-attributes.md)
* [Настройка синхронизации с помощью настраиваемого конечного атрибутов](../resources/synchronization-configure-with-custom-target-attributes.md)



