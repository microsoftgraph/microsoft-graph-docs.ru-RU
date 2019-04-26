---
title: Общие сведения об API синхронизации Azure AD
description: ') позволяет автоматизировать создание, Обслуживание и удаление удостоверений в приложениях Cloud (программное обеспечение, в качестве службы или SaaS), таких как Dropbox, Salesforce, ServiceNow и т. д. С помощью API синхронизации в Microsoft Graph можно управлять синхронизацией удостоверений программным способом, в том числе:'
localization_priority: Normal
ms.openlocfilehash: e472acc60e74c6a22a744d84e7e4dcf672337a6e
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342936"
---
# <a name="azure-ad-synchronization-api-overview"></a>Общие сведения об API синхронизации Azure AD

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Синхронизация удостоверений Azure Active Directory (также называемая "наполнением") позволяет автоматизировать создание, Обслуживание и удаление удостоверений в Cloud (программное обеспечение, в виде службы или SaaS), например Dropbox, Salesforce, ServiceNow и многое другое. С помощью API синхронизации в Microsoft Graph можно управлять синхронизацией удостоверений программным способом, в том числе:

- Создание, запуск и остановка заданий синхронизации
- Внесение изменений в схему синхронизации для заданий
- Проверка текущего состояния синхронизации 

Дополнительные сведения о синхронизации в Azure AD приведены в следующих статьях:

* [Автоматизация подготовки пользователей и их отмена в приложениях SaaS с помощью Azure Active Directory](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-saas-app-provisioning)
* [Управление предоставлением учетных записей пользователей для корпоративных приложений на портале Azure](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-enterprise-apps-manage-provisioning)

Вы также можете попробовать API в [проводнике Graph](https://developer.microsoft.com/graph/graph-explorer) в образце клиента или в собственном клиенте.

## <a name="synchronization-job"></a>Задание синхронизации

Задания синхронизации выполняют синхронизацию, периодически запуская в фоновом режиме, запрашивают изменения в одном каталоге и отправляют их в другой каталог. Задание синхронизации всегда относится к определенному экземпляру приложения в клиенте. В рамках настройки задания синхронизации необходимо предоставить авторизацию для чтения и записи объектов в целевом каталоге, а также для настройки схемы синхронизации задания.

Более подробную информацию можно узнать в статье [Задание синхронизации](synchronization-synchronizationjob.md).

## <a name="synchronization-schema"></a>Схема синхронизации

Схема синхронизации определяет объекты, которые будут синхронизированы и как они будут синхронизированы. Схема синхронизации содержит большую часть сведений о настройке для определенного задания синхронизации. Как правило, вы настраиваете некоторые [сопоставления атрибутов](synchronization-attributemapping.md)или добавляете [Фильтр областей](synchronization-filter.md) для синхронизации только объектов, удовлетворяющих определенному условию.

Схема синхронизации включает в себя следующие компоненты:

- Определения каталогов
- Правила синхронизации
- Сопоставления объектов

Более подробную информацию можно узнать в статье [схема синхронизации](synchronization-synchronizationschema.md).

## <a name="synchronization-template"></a>Шаблон синхронизации

Шаблон синхронизации предоставляет предварительно настроенные параметры синхронизации для определенного приложения. Эти параметры (наиболее важное, [схема синхронизации](synchronization-synchronizationschema.md)) будут использоваться по умолчанию для всех [заданий синхронизации](synchronization-synchronizationjob.md) , основанных на этом шаблоне. Шаблоны задаются разработчиком приложения.

Для получения дополнительных сведений см [шаблон синхронизации](synchronization-synchronizationtemplate.md).

## <a name="working-with-the-synchronization-api"></a>Работа с API синхронизации

Работа с API синхронизации в основном включает доступ к ресурсам [синчронизатионжоб](synchronization-synchronizationjob.md) и [синчронизатионсчема](synchronization-synchronizationschema.md) . Чтобы найти ресурс [синчронизатионжоб](synchronization-synchronizationjob.md) , необходимо знать идентификатор объекта участника службы, к которому относится задание синхронизации. В приведенных ниже примерах показано, как работать с ресурсами **синчронизатионжоб** и **синчронизатионсчема** .

### <a name="authorization"></a>Authorization

API синхронизации Azure AD использует OAuth 2,0 для проверки подлинности. Перед выполнением запросов к API необходимо получить маркер доступа. Дополнительные сведения [можно найти в статье получение маркеров доступа для вызова Microsoft Graph](https://developer.microsoft.com/graph/docs/concepts/auth_overview). Для доступа к ресурсам синхронизации приложению требуются разрешения Directory. ReadWrite. ALL. Для получения дополнительных сведений ознакомьтесь с разрешениями для [каталогов](/graph/permissions-reference#directory-permissions).

### <a name="find-the-service-principal-object-by-display-name"></a>Поиск объекта субъекта службы по отображаемому имени

В приведенном ниже примере показано, как найти объект участника службы по отображаемому имени.

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

### <a name="find-the-service-principal-object-by-app-id"></a>Поиск объекта субъекта службы по ИДЕНТИФИКАТОРу приложения

В приведенном ниже примере показано, как найти объект субъекта службы по ИДЕНТИФИКАТОРу приложения.

**Request** 
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

### <a name="list-existing-synchronization-jobs"></a>ПереЧисление существующих заданий синхронизации

В приведенном ниже примере показано, как перечислить существующие задания синхронизации.

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

### <a name="get-synchronization-job-status"></a>Получение состояния задания синхронизации
В приведенном ниже примере показано, как получить состояние задания синхронизации.

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

### <a name="get-synchronization-schema"></a>Получение схемы синхронизации
В приведенном ниже примере показано, как получить схему синхронизации.

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
* [Настройка синхронизации с пользовательскими целевыми атрибутами](../resources/synchronization-configure-with-custom-target-attributes.md)



