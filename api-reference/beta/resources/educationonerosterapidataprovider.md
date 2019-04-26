---
title: ресурс Едукатиононеростерапидатапровидер
description: Используется для настройки профиля синхронизации данных School при использовании API OneRoster в качестве источника входных данных.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 4ac232f71600f701efd8d085386fa9070773b475
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33334196"
---
# <a name="educationonerosterapidataprovider-resource"></a><span data-ttu-id="f1990-103">ресурс Едукатиононеростерапидатапровидер</span><span class="sxs-lookup"><span data-stu-id="f1990-103">educationOneRosterApiDataProvider resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f1990-104">Используется для настройки профиля синхронизации данных School при использовании [API OneRoster](https://www.imsglobal.org/activity/onerosterlis) в качестве источника входных данных.</span><span class="sxs-lookup"><span data-stu-id="f1990-104">Used to set up the school data synchronization profile when the [OneRoster API](https://www.imsglobal.org/activity/onerosterlis) is used as the input source.</span></span>

<span data-ttu-id="f1990-105">Производный от [едукатионсинчронизатиондатапровидер](educationsynchronizationdataprovider.md).</span><span class="sxs-lookup"><span data-stu-id="f1990-105">Derived from [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).</span></span>

## <a name="properties"></a><span data-ttu-id="f1990-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="f1990-106">Properties</span></span>

| <span data-ttu-id="f1990-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="f1990-107">Property</span></span> | <span data-ttu-id="f1990-108">Тип</span><span class="sxs-lookup"><span data-stu-id="f1990-108">Type</span></span> | <span data-ttu-id="f1990-109">Описание</span><span class="sxs-lookup"><span data-stu-id="f1990-109">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="f1990-110">**Коннектионурл**</span><span class="sxs-lookup"><span data-stu-id="f1990-110">**connectionUrl**</span></span> | <span data-ttu-id="f1990-111">String</span><span class="sxs-lookup"><span data-stu-id="f1990-111">String</span></span> | <span data-ttu-id="f1990-112">URL-адрес подключения к экземпляру OneRoster.</span><span class="sxs-lookup"><span data-stu-id="f1990-112">The connection URL to the OneRoster instance.</span></span> |
| <span data-ttu-id="f1990-113">**Счулсидс**</span><span class="sxs-lookup"><span data-stu-id="f1990-113">**schoolsIds**</span></span> | <span data-ttu-id="f1990-114">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="f1990-114">String collection</span></span> |  <span data-ttu-id="f1990-115">Список Саурцедидс School для синхронизации.</span><span class="sxs-lookup"><span data-stu-id="f1990-115">The list of school sourcedIds to sync.</span></span> |
| <span data-ttu-id="f1990-116">**providerName**</span><span class="sxs-lookup"><span data-stu-id="f1990-116">**providerName**</span></span> | <span data-ttu-id="f1990-117">String</span><span class="sxs-lookup"><span data-stu-id="f1990-117">String</span></span> | <span data-ttu-id="f1990-118">Имя поставщика службы OneRoster, как определено [спецификациЕй OneRoster](https://www.imsglobal.org/oneroster-v11-final-best-practice-and-implementation-guide#AppA).</span><span class="sxs-lookup"><span data-stu-id="f1990-118">The OneRoster Service Provider name as defined by the [OneRoster specification](https://www.imsglobal.org/oneroster-v11-final-best-practice-and-implementation-guide#AppA).</span></span> |
| <span data-ttu-id="f1990-119">**Коннектионсеттингс**</span><span class="sxs-lookup"><span data-stu-id="f1990-119">**connectionSettings**</span></span> | [<span data-ttu-id="f1990-120">Microsoft. Graph. Едукатионсинчронизатионконнектионсеттингс</span><span class="sxs-lookup"><span data-stu-id="f1990-120">microsoft.graph.educationSynchronizationConnectionSettings</span></span>](educationsynchronizationconnectionsettings.md) | <span data-ttu-id="f1990-121">Параметры подключения для экземпляра OneRoster.</span><span class="sxs-lookup"><span data-stu-id="f1990-121">Connection settings for the OneRoster instance.</span></span> <span data-ttu-id="f1990-122">Должен иметь тип [Microsoft. Graph. educationSynchronizationOAuth1ConnectionSettings](educationsynchronizationoauth1connectionsettings.md) или [Microsoft. Graph. educationSynchronizationOAuth2ClientCredentialsConnectionSettings](educationsynchronizationoauth2clientcredentialsconnectionsettings.md).</span><span class="sxs-lookup"><span data-stu-id="f1990-122">Should be of type [microsoft.graph.educationSynchronizationOAuth1ConnectionSettings](educationsynchronizationoauth1connectionsettings.md) or [microsoft.graph.educationSynchronizationOAuth2ClientCredentialsConnectionSettings](educationsynchronizationoauth2clientcredentialsconnectionsettings.md).</span></span> |
| <span data-ttu-id="f1990-123">**настроек**</span><span class="sxs-lookup"><span data-stu-id="f1990-123">**customizations**</span></span> | [<span data-ttu-id="f1990-124">Microsoft. Graph. Едукатионсинчронизатионкустомизатионс</span><span class="sxs-lookup"><span data-stu-id="f1990-124">microsoft.graph.educationSynchronizationCustomizations</span></span>](educationsynchronizationcustomizations.md) | <span data-ttu-id="f1990-125">НеОбязательная Настройка, применяемая к профилю синхронизации.</span><span class="sxs-lookup"><span data-stu-id="f1990-125">Optional customization to be applied to the synchronization profile.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f1990-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f1990-126">JSON representation</span></span>
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
