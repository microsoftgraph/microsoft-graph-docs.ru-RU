---
title: Тип ресурса Сервицеусеражент
description: Тип Сервицеусеражент
localization_priority: Normal
author: stephenjust
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 052c177e2cef4adf5a882408c3cdef3a211dea73
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48069332"
---
# <a name="serviceuseragent-resource-type"></a><span data-ttu-id="54060-103">Тип ресурса Сервицеусеражент</span><span class="sxs-lookup"><span data-stu-id="54060-103">serviceUserAgent resource type</span></span>

<span data-ttu-id="54060-104">Пространство имен: microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="54060-104">Namespace: microsoft.graph.callRecords</span></span>

<span data-ttu-id="54060-105">Представляет агент пользователя службы конечной точки в вызове.</span><span class="sxs-lookup"><span data-stu-id="54060-105">Represents a service user agent of an endpoint in a call.</span></span> <span data-ttu-id="54060-106">Наследуется от типа [UserAgent](callrecords-useragent.md) .</span><span class="sxs-lookup"><span data-stu-id="54060-106">Inherits from [userAgent](callrecords-useragent.md) type.</span></span>

## <a name="properties"></a><span data-ttu-id="54060-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="54060-107">Properties</span></span>

| <span data-ttu-id="54060-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="54060-108">Property</span></span>     | <span data-ttu-id="54060-109">Тип</span><span class="sxs-lookup"><span data-stu-id="54060-109">Type</span></span>        | <span data-ttu-id="54060-110">Описание</span><span class="sxs-lookup"><span data-stu-id="54060-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="54060-111">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="54060-111">applicationVersion</span></span>|<span data-ttu-id="54060-112">String</span><span class="sxs-lookup"><span data-stu-id="54060-112">String</span></span>|<span data-ttu-id="54060-113">Определяет версию программного обеспечения приложения, используемого конечной точкой.</span><span class="sxs-lookup"><span data-stu-id="54060-113">Identifies the version of application software used by this endpoint.</span></span>|
|<span data-ttu-id="54060-114">headerValue</span><span class="sxs-lookup"><span data-stu-id="54060-114">headerValue</span></span>|<span data-ttu-id="54060-115">Строка</span><span class="sxs-lookup"><span data-stu-id="54060-115">String</span></span>|<span data-ttu-id="54060-116">Значение заголовка User — Agent, указанное конечной точкой.</span><span class="sxs-lookup"><span data-stu-id="54060-116">User-agent header value reported by this endpoint.</span></span>|
|<span data-ttu-id="54060-117">role</span><span class="sxs-lookup"><span data-stu-id="54060-117">role</span></span>|<span data-ttu-id="54060-118">Microsoft. Graph. Каллрекордс. Сервицероле</span><span class="sxs-lookup"><span data-stu-id="54060-118">microsoft.graph.callRecords.serviceRole</span></span>|<span data-ttu-id="54060-119">Определяет роль службы, используемой этой конечной точкой.</span><span class="sxs-lookup"><span data-stu-id="54060-119">Identifies the role of the service used by this endpoint.</span></span> <span data-ttu-id="54060-120">Возможные значения: `unknown` ,,,,,,,,,,,,,,,,,,,,,,,,,,, `customBot` `skypeForBusinessMicrosoftTeamsGateway` `skypeForBusinessAudioVideoMcu` `skypeForBusinessApplicationSharingMcu` `skypeForBusinessCallQueues` `skypeForBusinessAutoAttendant` `mediationServer` `mediationServerCloudConnectorEdition` `exchangeUnifiedMessagingService` `mediaController` `conferencingAnnouncementService` `conferencingAttendant` `audioTeleconferencerController` `skypeForBusinessUnifiedCommunicationApplicationPlatform` `responseGroupServiceAnnouncementService` `gateway` `skypeTranslator` `skypeForBusinessAttendant` `responseGroupService` `voicemail` `unknownFutureValue` .</span><span class="sxs-lookup"><span data-stu-id="54060-120">Possible values are: `unknown`, `customBot`, `skypeForBusinessMicrosoftTeamsGateway`, `skypeForBusinessAudioVideoMcu`, `skypeForBusinessApplicationSharingMcu`, `skypeForBusinessCallQueues`, `skypeForBusinessAutoAttendant`, `mediationServer`, `mediationServerCloudConnectorEdition`, `exchangeUnifiedMessagingService`, `mediaController`, `conferencingAnnouncementService`, `conferencingAttendant`, `audioTeleconferencerController`, `skypeForBusinessUnifiedCommunicationApplicationPlatform`, `responseGroupServiceAnnouncementService`, `gateway`, `skypeTranslator`, `skypeForBusinessAttendant`, `responseGroupService`, `voicemail`, `unknownFutureValue`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="54060-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="54060-121">JSON representation</span></span>

<span data-ttu-id="54060-122">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="54060-122">The following is a JSON representation of the resource.</span></span>

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
