---
title: Тип ресурса Сервицеусеражент
description: Тип Сервицеусеражент
localization_priority: Normal
author: stephenjust
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 8e411b7170f99f57eac4cdb7c56cfc64bcf2aee5
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/02/2020
ms.locfileid: "44491177"
---
# <a name="serviceuseragent-resource-type"></a><span data-ttu-id="ff9a6-103">Тип ресурса Сервицеусеражент</span><span class="sxs-lookup"><span data-stu-id="ff9a6-103">serviceUserAgent resource type</span></span>

<span data-ttu-id="ff9a6-104">Пространство имен: microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="ff9a6-104">Namespace: microsoft.graph.callRecords</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ff9a6-105">Представляет агент пользователя службы конечной точки в вызове.</span><span class="sxs-lookup"><span data-stu-id="ff9a6-105">Represents a service user agent of an endpoint in a call.</span></span> <span data-ttu-id="ff9a6-106">Наследуется от типа [UserAgent](callrecords-useragent.md) .</span><span class="sxs-lookup"><span data-stu-id="ff9a6-106">Inherits from [userAgent](callrecords-useragent.md) type.</span></span>

## <a name="properties"></a><span data-ttu-id="ff9a6-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="ff9a6-107">Properties</span></span>

| <span data-ttu-id="ff9a6-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="ff9a6-108">Property</span></span>     | <span data-ttu-id="ff9a6-109">Тип</span><span class="sxs-lookup"><span data-stu-id="ff9a6-109">Type</span></span>        | <span data-ttu-id="ff9a6-110">Описание</span><span class="sxs-lookup"><span data-stu-id="ff9a6-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ff9a6-111">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="ff9a6-111">applicationVersion</span></span>|<span data-ttu-id="ff9a6-112">String</span><span class="sxs-lookup"><span data-stu-id="ff9a6-112">String</span></span>|<span data-ttu-id="ff9a6-113">Определяет версию программного обеспечения приложения, используемого конечной точкой.</span><span class="sxs-lookup"><span data-stu-id="ff9a6-113">Identifies the version of application software used by this endpoint.</span></span>|
|<span data-ttu-id="ff9a6-114">headerValue</span><span class="sxs-lookup"><span data-stu-id="ff9a6-114">headerValue</span></span>|<span data-ttu-id="ff9a6-115">String</span><span class="sxs-lookup"><span data-stu-id="ff9a6-115">String</span></span>|<span data-ttu-id="ff9a6-116">Значение заголовка User — Agent, указанное конечной точкой.</span><span class="sxs-lookup"><span data-stu-id="ff9a6-116">User-agent header value reported by this endpoint.</span></span>|
|<span data-ttu-id="ff9a6-117">role</span><span class="sxs-lookup"><span data-stu-id="ff9a6-117">role</span></span>|<span data-ttu-id="ff9a6-118">Microsoft. Graph. Каллрекордс. Сервицероле</span><span class="sxs-lookup"><span data-stu-id="ff9a6-118">microsoft.graph.callRecords.serviceRole</span></span>|<span data-ttu-id="ff9a6-119">Определяет роль службы, используемой этой конечной точкой.</span><span class="sxs-lookup"><span data-stu-id="ff9a6-119">Identifies the role of the service used by this endpoint.</span></span> <span data-ttu-id="ff9a6-120">Возможные значения: `unknown` ,,,,,,,,,,,,,,,,,,,,,,,,,,, `customBot` `skypeForBusinessMicrosoftTeamsGateway` `skypeForBusinessAudioVideoMcu` `skypeForBusinessApplicationSharingMcu` `skypeForBusinessCallQueues` `skypeForBusinessAutoAttendant` `mediationServer` `mediationServerCloudConnectorEdition` `exchangeUnifiedMessagingService` `mediaController` `conferencingAnnouncementService` `conferencingAttendant` `audioTeleconferencerController` `skypeForBusinessUnifiedCommunicationApplicationPlatform` `responseGroupServiceAnnouncementService` `gateway` `skypeTranslator` `skypeForBusinessAttendant` `responseGroupService` `voicemail` `unknownFutureValue` .</span><span class="sxs-lookup"><span data-stu-id="ff9a6-120">Possible values are: `unknown`, `customBot`, `skypeForBusinessMicrosoftTeamsGateway`, `skypeForBusinessAudioVideoMcu`, `skypeForBusinessApplicationSharingMcu`, `skypeForBusinessCallQueues`, `skypeForBusinessAutoAttendant`, `mediationServer`, `mediationServerCloudConnectorEdition`, `exchangeUnifiedMessagingService`, `mediaController`, `conferencingAnnouncementService`, `conferencingAttendant`, `audioTeleconferencerController`, `skypeForBusinessUnifiedCommunicationApplicationPlatform`, `responseGroupServiceAnnouncementService`, `gateway`, `skypeTranslator`, `skypeForBusinessAttendant`, `responseGroupService`, `voicemail`, `unknownFutureValue`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ff9a6-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ff9a6-121">JSON representation</span></span>

<span data-ttu-id="ff9a6-122">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ff9a6-122">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callRecords.serviceUserAgent",
  "baseType": "microsoft.graph.callRecords.userAgent"
}-->

```json
{
  "applicationVersion": "String",
  "headerValue": "String",
  "role": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "serviceUserAgent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->