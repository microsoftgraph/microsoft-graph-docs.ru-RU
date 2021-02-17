---
title: Обзор API синхронизации Azure AD
description: Автоматизация предоставления удостоверений из систем управления персоналом, Active Directory и Azure Active Directory в облачные приложения.
localization_priority: Normal
doc_type: conceptualPageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: 2c0cbfae55ca02743d1b8e10777580e431529103
ms.sourcegitcommit: 42fdb068616222eb6b0813e93b33e830fc7eedc0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/17/2021
ms.locfileid: "50272516"
---
# <a name="azure-ad-synchronization-api-overview"></a>Обзор API синхронизации Azure AD

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Синхронизация удостоверений Azure Active Directory (Azure AD) (также называемая "подготовка") позволяет автоматизировать подготовка (создание, обслуживание) и отмену (удаление) удостоверений из любого из следующих систем:
- Из Active Directory в Azure AD
- Рабочий день в Azure AD
- Azure AD для облачных приложений, таких как Dropbox, Salesforce, ServiceNow и другие 

Можно воспользоваться интерфейсами API синхронизации в Microsoft Graph для управления синхронизацией удостоверений программными средствами, в том числе для:

- создания, запуска и остановки заданий синхронизации
- изменения схемы синхронизации для заданий
- проверки текущего состояния синхронизации

Дополнительные сведения о синхронизации в Azure AD см. в:

* [Автоматизация пользовательской подготовка и подготовка к приложениям SaaS с помощью Azure Active Directory](/azure/active-directory/active-directory-saas-app-provisioning)
* [Управление подготовкаю учетных записей пользователей для корпоративных приложений на портале Azure](/azure/active-directory/active-directory-enterprise-apps-manage-provisioning)

Вы также можете попробовать API в обозревателе [Graph](https://developer.microsoft.com/graph/graph-explorer) в примере клиента или собственном клиенте.

## <a name="synchronization-job"></a>Задание синхронизации

Задания синхронизации выполняют синхронизацию, периодически работая в фоновом режиме, выполняя опрос изменений в одном каталоге и перенажимая их в другой каталог. Задание синхронизации всегда является специфическим для конкретного экземпляра приложения в клиенте. В рамках настройки задания синхронизации необходимо предоставить авторизацию для чтения и записи объектов в целевом каталоге и настроить схему синхронизации задания.

Дополнительные сведения см. [в заданиях синхронизации.](synchronization-synchronizationjob.md)

## <a name="synchronization-schema"></a>Схема синхронизации

Схема синхронизации определяет, какие объекты будут синхронизироваться и как они будут синхронизироваться. Схема синхронизации содержит большую часть сведений об установке для конкретного задания синхронизации. Как правило, некоторые сопоставления [](synchronization-attributemapping.md)атрибутов настраиваются или [](synchronization-filter.md) добавляются фильтры области для синхронизации только объектов, удовлетворяющих определенному условию.

Схема синхронизации включает следующие компоненты:

- Определения каталогов
- Правила синхронизации
- Сопоставления объектов

Дополнительные сведения см. [в схеме синхронизации.](synchronization-synchronizationschema.md)

## <a name="synchronization-template"></a>Шаблон синхронизации

Шаблон синхронизации предоставляет предварительно настроенные параметры синхронизации для конкретного приложения. Эти параметры (что самое важное, схема синхронизации) [](synchronization-synchronizationjob.md) будут использоваться по умолчанию для любого задания синхронизации, основанного на шаблоне. [](synchronization-synchronizationschema.md) Шаблоны заданы разработчиком приложения.

Дополнительные сведения см. [в шаблоне синхронизации.](synchronization-synchronizationtemplate.md)

## <a name="working-with-the-synchronization-api"></a>Работа с API синхронизации

Работа с API синхронизации в основном включает доступ к ресурсам [synchronizationJob](synchronization-synchronizationjob.md) и [synchronizationSchema.](synchronization-synchronizationschema.md) Чтобы найти ресурс [synchronizationJob,](synchronization-synchronizationjob.md) необходимо знать ИД объекта-службы, к которой принадлежит задание синхронизации. В следующих примерах покажем, как работать с **ресурсами synchronizationJob** и **synchronizationSchema.**

### <a name="authorization"></a>Authorization

Для авторизации API синхронизации Azure AD использует OAuth 2.0. Прежде чем делать запросы к API, необходимо получить маркер доступа. Дополнительные сведения см. в сведениях о [том, как получить маркеры доступа для вызова Microsoft Graph.](/graph/auth/) Для доступа к ресурсам синхронизации приложению необходимы разрешения Directory.ReadWrite.All. Дополнительные сведения [см. в сведениях о разрешениях для каталогов.](/graph/permissions-reference#directory-permissions)

### <a name="find-the-service-principal-object-by-display-name"></a>Поиск объекта-службы по отображаемой имени

В следующем примере показано, как найти объект-службу по отображаемой имени.

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
   "value":[
      {
         "id":"bc0dc311-87df-48ac-91b1-259bd2c3a31c",
         "appId":"f7808c5e-cb57-4e37-8094-406d302c0f8d",
         "displayName":"Salesforce"
      },
      {
         "id":"d813d7d7-0f41-4edc-b284-d0dfaf399d15",
         "appId":"219561ee-1480-4c67-9aa6-63d861fae3ef",
         "displayName":"salesforce 3"
      }
   ]
}
```

### <a name="find-the-service-principal-object-by-app-id"></a>Поиск объекта-службы по ИД приложения

В следующем примере показано, как найти объект-службу по ИД приложения.

**Запрос**
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/servicePrincipals?$select=id,appId,displayName&$filter=AppId eq '219561ee-1480-4c67-9aa6-63d861fae3ef'
```

**Отклик**
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

В следующем примере показано, как перечислить существующие задания синхронизации.

**Запрос**
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs
GET https://graph.microsoft.com/beta/servicePrincipals/60443998-8cf7-4e61-b05c-a53b658cb5e1/synchronization/jobs
```

**Отклик**
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

### <a name="get-synchronization-job-status"></a>Получить состояние задания синхронизации
В следующем примере показано, как получить состояние задания синхронизации.

**Запрос**
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}

GET https://graph.microsoft.com/beta/servicePrincipals/60443998-8cf7-4e61-b05c-a53b658cb5e1/synchronization/jobs/SfSandboxOutDelta.e4bbf44533ea4eabb17027f3a92e92aa
```

**Отклик**
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

### <a name="get-synchronization-schema"></a>Получить схему синхронизации
В следующем примере показано, как получить схему синхронизации.

**Запрос**
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
```

**Отклик**
<!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK

{
    "directories": [],
    "synchronizationRules": []
}
```
## <a name="see-also"></a>См. также

* [Настройка синхронизации с атрибутами расширения каталога](../resources/synchronization-configure-with-directory-extension-attributes.md)
* [Настройка синхронизации с настраиваемых целевых атрибутов](../resources/synchronization-configure-with-custom-target-attributes.md)
