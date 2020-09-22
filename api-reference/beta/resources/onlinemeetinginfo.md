---
title: Тип ресурса Онлинемитингинфо
description: Сведения, необходимые участнику, чтобы присоединиться к собранию по сети.
localization_priority: Normal
author: ananmishr
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: fb971295919f779c3faddb34ceeb96d531011b1f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48052574"
---
# <a name="onlinemeetinginfo-resource-type"></a><span data-ttu-id="10916-103">Тип ресурса Онлинемитингинфо</span><span class="sxs-lookup"><span data-stu-id="10916-103">onlineMeetingInfo resource type</span></span>

<span data-ttu-id="10916-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="10916-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="10916-105">Сведения, необходимые участнику, чтобы присоединиться к собранию по сети.</span><span class="sxs-lookup"><span data-stu-id="10916-105">Details for an attendee to join the meeting online.</span></span>

## <a name="properties"></a><span data-ttu-id="10916-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="10916-106">Properties</span></span>

| <span data-ttu-id="10916-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="10916-107">Property</span></span>     | <span data-ttu-id="10916-108">Тип</span><span class="sxs-lookup"><span data-stu-id="10916-108">Type</span></span>        | <span data-ttu-id="10916-109">Описание</span><span class="sxs-lookup"><span data-stu-id="10916-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="10916-110">конференцеид</span><span class="sxs-lookup"><span data-stu-id="10916-110">conferenceId</span></span>|<span data-ttu-id="10916-111">String</span><span class="sxs-lookup"><span data-stu-id="10916-111">String</span></span>| <span data-ttu-id="10916-112">Идентификатор конференции.</span><span class="sxs-lookup"><span data-stu-id="10916-112">The ID of the conference.</span></span>|
|<span data-ttu-id="10916-113">жоинурл</span><span class="sxs-lookup"><span data-stu-id="10916-113">joinUrl</span></span>|<span data-ttu-id="10916-114">String</span><span class="sxs-lookup"><span data-stu-id="10916-114">String</span></span>| <span data-ttu-id="10916-115">Внешняя ссылка, которая запускает собрание по сети.</span><span class="sxs-lookup"><span data-stu-id="10916-115">The external link that launches the online meeting.</span></span> <span data-ttu-id="10916-116">Это URL-адрес, который клиенты будут запускать в браузере и перенаправит пользователя для присоединения к собранию.</span><span class="sxs-lookup"><span data-stu-id="10916-116">This is a URL that clients will launch into a browser and will redirect the user to join the meeting.</span></span>|
|<span data-ttu-id="10916-117">phones</span><span class="sxs-lookup"><span data-stu-id="10916-117">phones</span></span>|<span data-ttu-id="10916-118">Коллекция [phone](phone.md)</span><span class="sxs-lookup"><span data-stu-id="10916-118">[phone](phone.md) collection</span></span>| <span data-ttu-id="10916-119">Все номера телефонов, связанные с этой Конференции.</span><span class="sxs-lookup"><span data-stu-id="10916-119">All of the phone numbers associated with this conference.</span></span>|
|<span data-ttu-id="10916-120">куиккдиал</span><span class="sxs-lookup"><span data-stu-id="10916-120">quickDial</span></span>|<span data-ttu-id="10916-121">String</span><span class="sxs-lookup"><span data-stu-id="10916-121">String</span></span>| <span data-ttu-id="10916-122">Предварительно отформатированный куиккдиал для этого вызова.</span><span class="sxs-lookup"><span data-stu-id="10916-122">The pre-formatted quickdial for this call.</span></span>|
|<span data-ttu-id="10916-123">толлфринумберс</span><span class="sxs-lookup"><span data-stu-id="10916-123">tollFreeNumbers</span></span>|<span data-ttu-id="10916-124">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="10916-124">String collection</span></span>| <span data-ttu-id="10916-125">Бесплатных бесплатных номеров, которые можно использовать для присоединения к Конференции.</span><span class="sxs-lookup"><span data-stu-id="10916-125">The toll free numbers that can be used to join the conference.</span></span>|
|<span data-ttu-id="10916-126">толлнумбер</span><span class="sxs-lookup"><span data-stu-id="10916-126">tollNumber</span></span>|<span data-ttu-id="10916-127">String</span><span class="sxs-lookup"><span data-stu-id="10916-127">String</span></span>| <span data-ttu-id="10916-128">Платный номер, который можно использовать для присоединения к Конференции.</span><span class="sxs-lookup"><span data-stu-id="10916-128">The toll number that can be used to join the conference.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="10916-129">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="10916-129">JSON representation</span></span>

<span data-ttu-id="10916-130">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="10916-130">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.onlineMeetingInfo"
}-->

```json
{
  "conferenceId": "String",
  "joinUrl": "String",
  "phones": [{"@odata.type": "microsoft.graph.phone"}],
  "quickDial": "String",
  "tollFreeNumbers": ["String"],
  "tollNumber": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onlineMeetingInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->s


