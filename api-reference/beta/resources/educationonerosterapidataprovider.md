---
title: ресурс Едукатиононеростерапидатапровидер
description: Используется для настройки профиля синхронизации данных School при использовании API OneRoster в качестве источника входных данных.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: ca3341c84b79ff25e55be1abf5a8a5a031e84b02
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2020
ms.locfileid: "44290387"
---
# <a name="educationonerosterapidataprovider-resource"></a><span data-ttu-id="bf6c0-103">ресурс Едукатиононеростерапидатапровидер</span><span class="sxs-lookup"><span data-stu-id="bf6c0-103">educationOneRosterApiDataProvider resource</span></span>

<span data-ttu-id="bf6c0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bf6c0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bf6c0-105">Используется для настройки профиля синхронизации данных School при использовании [API OneRoster](https://www.imsglobal.org/activity/onerosterlis) в качестве источника входных данных.</span><span class="sxs-lookup"><span data-stu-id="bf6c0-105">Used to set up the school data synchronization profile when the [OneRoster API](https://www.imsglobal.org/activity/onerosterlis) is used as the input source.</span></span>

<span data-ttu-id="bf6c0-106">Производный от [едукатионсинчронизатиондатапровидер](educationsynchronizationdataprovider.md).</span><span class="sxs-lookup"><span data-stu-id="bf6c0-106">Derived from [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).</span></span>

## <a name="properties"></a><span data-ttu-id="bf6c0-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="bf6c0-107">Properties</span></span>

| <span data-ttu-id="bf6c0-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="bf6c0-108">Property</span></span> | <span data-ttu-id="bf6c0-109">Тип</span><span class="sxs-lookup"><span data-stu-id="bf6c0-109">Type</span></span> | <span data-ttu-id="bf6c0-110">Описание</span><span class="sxs-lookup"><span data-stu-id="bf6c0-110">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="bf6c0-111">**коннектионурл**</span><span class="sxs-lookup"><span data-stu-id="bf6c0-111">**connectionUrl**</span></span> | <span data-ttu-id="bf6c0-112">String</span><span class="sxs-lookup"><span data-stu-id="bf6c0-112">String</span></span> | <span data-ttu-id="bf6c0-113">URL-адрес подключения к экземпляру OneRoster.</span><span class="sxs-lookup"><span data-stu-id="bf6c0-113">The connection URL to the OneRoster instance.</span></span> |
| <span data-ttu-id="bf6c0-114">**счулсидс**</span><span class="sxs-lookup"><span data-stu-id="bf6c0-114">**schoolsIds**</span></span> | <span data-ttu-id="bf6c0-115">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="bf6c0-115">String collection</span></span> |  <span data-ttu-id="bf6c0-116">Список Саурцедидс School для синхронизации.</span><span class="sxs-lookup"><span data-stu-id="bf6c0-116">The list of school sourcedIds to sync.</span></span> |
| <span data-ttu-id="bf6c0-117">**providerName**</span><span class="sxs-lookup"><span data-stu-id="bf6c0-117">**providerName**</span></span> | <span data-ttu-id="bf6c0-118">String</span><span class="sxs-lookup"><span data-stu-id="bf6c0-118">String</span></span> | <span data-ttu-id="bf6c0-119">Имя поставщика службы OneRoster, как определено [спецификацией OneRoster](https://www.imsglobal.org/oneroster-v11-final-best-practice-and-implementation-guide#AppA).</span><span class="sxs-lookup"><span data-stu-id="bf6c0-119">The OneRoster Service Provider name as defined by the [OneRoster specification](https://www.imsglobal.org/oneroster-v11-final-best-practice-and-implementation-guide#AppA).</span></span> |
| <span data-ttu-id="bf6c0-120">**коннектионсеттингс**</span><span class="sxs-lookup"><span data-stu-id="bf6c0-120">**connectionSettings**</span></span> | [<span data-ttu-id="bf6c0-121">Microsoft. Graph. Едукатионсинчронизатионконнектионсеттингс</span><span class="sxs-lookup"><span data-stu-id="bf6c0-121">microsoft.graph.educationSynchronizationConnectionSettings</span></span>](educationsynchronizationconnectionsettings.md) | <span data-ttu-id="bf6c0-122">Параметры подключения для экземпляра OneRoster.</span><span class="sxs-lookup"><span data-stu-id="bf6c0-122">Connection settings for the OneRoster instance.</span></span> <span data-ttu-id="bf6c0-123">Должен иметь тип [Microsoft. Graph. educationSynchronizationOAuth1ConnectionSettings](educationsynchronizationoauth1connectionsettings.md) или [Microsoft. Graph. educationSynchronizationOAuth2ClientCredentialsConnectionSettings](educationsynchronizationoauth2clientcredentialsconnectionsettings.md).</span><span class="sxs-lookup"><span data-stu-id="bf6c0-123">Should be of type [microsoft.graph.educationSynchronizationOAuth1ConnectionSettings](educationsynchronizationoauth1connectionsettings.md) or [microsoft.graph.educationSynchronizationOAuth2ClientCredentialsConnectionSettings](educationsynchronizationoauth2clientcredentialsconnectionsettings.md).</span></span> |
| <span data-ttu-id="bf6c0-124">**настроек**</span><span class="sxs-lookup"><span data-stu-id="bf6c0-124">**customizations**</span></span> | [<span data-ttu-id="bf6c0-125">Microsoft. Graph. Едукатионсинчронизатионкустомизатионс</span><span class="sxs-lookup"><span data-stu-id="bf6c0-125">microsoft.graph.educationSynchronizationCustomizations</span></span>](educationsynchronizationcustomizations.md) | <span data-ttu-id="bf6c0-126">Необязательная настройка, применяемая к профилю синхронизации.</span><span class="sxs-lookup"><span data-stu-id="bf6c0-126">Optional customization to be applied to the synchronization profile.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bf6c0-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bf6c0-127">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationoneRosterApiDataProvider"
}-->

```json
{
    "@odata.type": "microsoft.graph.educationoneRosterApiDataProvider",
    "connectionUrl": "String",
    "providerName": "String",
    "schoolsIds": [
        "String"
    ],
    "connectionSettings": {
        "@odata.type": "microsoft.graph.educationSynchronizationOAuth1ConnectionSettings",
        "clientId": "String",
        "clientSecret": "String",
    },
    "customizations": { "@odata.type": "microsoft.graph.educationSynchronizationCustomizations" }
}
```
<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2020-05-06 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationOneRosterApiDataProvider resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
      "Error: microsoft.graph.educationoneRosterApiDataProvider/connectionSettings:\r\n      Referenced type microsoft.graph.educationSynchronizationConnectionSettings is not defined in the doc set! Potential suggestion: microsoft.graph.settings"
  ]
}-->