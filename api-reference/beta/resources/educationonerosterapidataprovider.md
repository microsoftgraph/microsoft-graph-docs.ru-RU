---
title: ресурс Едукатиононеростерапидатапровидер
description: Используется для настройки профиля синхронизации данных School при использовании API OneRoster в качестве источника входных данных.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: ca94043fdf215d47a1ccaf16f3a667f1178c1d57
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972637"
---
# <a name="educationonerosterapidataprovider-resource"></a><span data-ttu-id="a10f7-103">ресурс Едукатиононеростерапидатапровидер</span><span class="sxs-lookup"><span data-stu-id="a10f7-103">educationOneRosterApiDataProvider resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a10f7-104">Используется для настройки профиля синхронизации данных School при использовании [API OneRoster](https://www.imsglobal.org/activity/onerosterlis) в качестве источника входных данных.</span><span class="sxs-lookup"><span data-stu-id="a10f7-104">Used to set up the school data synchronization profile when the [OneRoster API](https://www.imsglobal.org/activity/onerosterlis) is used as the input source.</span></span>

<span data-ttu-id="a10f7-105">Производный от [едукатионсинчронизатиондатапровидер](educationsynchronizationdataprovider.md).</span><span class="sxs-lookup"><span data-stu-id="a10f7-105">Derived from [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).</span></span>

## <a name="properties"></a><span data-ttu-id="a10f7-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="a10f7-106">Properties</span></span>

| <span data-ttu-id="a10f7-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="a10f7-107">Property</span></span> | <span data-ttu-id="a10f7-108">Тип</span><span class="sxs-lookup"><span data-stu-id="a10f7-108">Type</span></span> | <span data-ttu-id="a10f7-109">Описание</span><span class="sxs-lookup"><span data-stu-id="a10f7-109">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="a10f7-110">**Коннектионурл**</span><span class="sxs-lookup"><span data-stu-id="a10f7-110">**connectionUrl**</span></span> | <span data-ttu-id="a10f7-111">String</span><span class="sxs-lookup"><span data-stu-id="a10f7-111">String</span></span> | <span data-ttu-id="a10f7-112">URL-адрес подключения к экземпляру OneRoster.</span><span class="sxs-lookup"><span data-stu-id="a10f7-112">The connection URL to the OneRoster instance.</span></span> |
| <span data-ttu-id="a10f7-113">**Счулсидс**</span><span class="sxs-lookup"><span data-stu-id="a10f7-113">**schoolsIds**</span></span> | <span data-ttu-id="a10f7-114">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="a10f7-114">String collection</span></span> |  <span data-ttu-id="a10f7-115">Список Саурцедидс School для синхронизации.</span><span class="sxs-lookup"><span data-stu-id="a10f7-115">The list of school sourcedIds to sync.</span></span> |
| <span data-ttu-id="a10f7-116">**providerName**</span><span class="sxs-lookup"><span data-stu-id="a10f7-116">**providerName**</span></span> | <span data-ttu-id="a10f7-117">String</span><span class="sxs-lookup"><span data-stu-id="a10f7-117">String</span></span> | <span data-ttu-id="a10f7-118">Имя поставщика службы OneRoster, как определено [спецификацией OneRoster](https://www.imsglobal.org/oneroster-v11-final-best-practice-and-implementation-guide#AppA).</span><span class="sxs-lookup"><span data-stu-id="a10f7-118">The OneRoster Service Provider name as defined by the [OneRoster specification](https://www.imsglobal.org/oneroster-v11-final-best-practice-and-implementation-guide#AppA).</span></span> |
| <span data-ttu-id="a10f7-119">**Коннектионсеттингс**</span><span class="sxs-lookup"><span data-stu-id="a10f7-119">**connectionSettings**</span></span> | [<span data-ttu-id="a10f7-120">Microsoft. Graph. Едукатионсинчронизатионконнектионсеттингс</span><span class="sxs-lookup"><span data-stu-id="a10f7-120">microsoft.graph.educationSynchronizationConnectionSettings</span></span>](educationsynchronizationconnectionsettings.md) | <span data-ttu-id="a10f7-121">Параметры подключения для экземпляра OneRoster.</span><span class="sxs-lookup"><span data-stu-id="a10f7-121">Connection settings for the OneRoster instance.</span></span> <span data-ttu-id="a10f7-122">Должен иметь тип [Microsoft. Graph. educationSynchronizationOAuth1ConnectionSettings](educationsynchronizationoauth1connectionsettings.md) или [Microsoft. Graph. educationSynchronizationOAuth2ClientCredentialsConnectionSettings](educationsynchronizationoauth2clientcredentialsconnectionsettings.md).</span><span class="sxs-lookup"><span data-stu-id="a10f7-122">Should be of type [microsoft.graph.educationSynchronizationOAuth1ConnectionSettings](educationsynchronizationoauth1connectionsettings.md) or [microsoft.graph.educationSynchronizationOAuth2ClientCredentialsConnectionSettings](educationsynchronizationoauth2clientcredentialsconnectionsettings.md).</span></span> |
| <span data-ttu-id="a10f7-123">**настроек**</span><span class="sxs-lookup"><span data-stu-id="a10f7-123">**customizations**</span></span> | [<span data-ttu-id="a10f7-124">Microsoft. Graph. Едукатионсинчронизатионкустомизатионс</span><span class="sxs-lookup"><span data-stu-id="a10f7-124">microsoft.graph.educationSynchronizationCustomizations</span></span>](educationsynchronizationcustomizations.md) | <span data-ttu-id="a10f7-125">Необязательная настройка, применяемая к профилю синхронизации.</span><span class="sxs-lookup"><span data-stu-id="a10f7-125">Optional customization to be applied to the synchronization profile.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a10f7-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a10f7-126">JSON representation</span></span>
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
