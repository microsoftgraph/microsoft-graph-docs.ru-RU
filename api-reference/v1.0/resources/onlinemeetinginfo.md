---
title: Тип ресурса Онлинемитингинфо
description: Сведения, необходимые участнику, чтобы присоединиться к собранию по сети.
localization_priority: Normal
author: ananmishr
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 063f2f43f98d9f2d75822f712c4e17755bc290f7
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2020
ms.locfileid: "43229453"
---
# <a name="onlinemeetinginfo-resource-type"></a><span data-ttu-id="f8746-103">Тип ресурса Онлинемитингинфо</span><span class="sxs-lookup"><span data-stu-id="f8746-103">onlineMeetingInfo resource type</span></span>

<span data-ttu-id="f8746-104">Сведения, необходимые участнику, чтобы присоединиться к собранию по сети.</span><span class="sxs-lookup"><span data-stu-id="f8746-104">Details for an attendee to join the meeting online.</span></span>

## <a name="properties"></a><span data-ttu-id="f8746-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="f8746-105">Properties</span></span>

| <span data-ttu-id="f8746-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="f8746-106">Property</span></span>     | <span data-ttu-id="f8746-107">Тип</span><span class="sxs-lookup"><span data-stu-id="f8746-107">Type</span></span>        | <span data-ttu-id="f8746-108">Описание</span><span class="sxs-lookup"><span data-stu-id="f8746-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f8746-109">конференцеид</span><span class="sxs-lookup"><span data-stu-id="f8746-109">conferenceId</span></span>|<span data-ttu-id="f8746-110">String</span><span class="sxs-lookup"><span data-stu-id="f8746-110">String</span></span>| <span data-ttu-id="f8746-111">Идентификатор конференции.</span><span class="sxs-lookup"><span data-stu-id="f8746-111">The ID of the conference.</span></span>|
|<span data-ttu-id="f8746-112">жоинурл</span><span class="sxs-lookup"><span data-stu-id="f8746-112">joinUrl</span></span>|<span data-ttu-id="f8746-113">String</span><span class="sxs-lookup"><span data-stu-id="f8746-113">String</span></span>| <span data-ttu-id="f8746-114">Внешняя ссылка, которая запускает собрание по сети.</span><span class="sxs-lookup"><span data-stu-id="f8746-114">The external link that launches the online meeting.</span></span> <span data-ttu-id="f8746-115">Это URL-адрес, который клиенты будут запускать в браузере и перенаправит пользователя для присоединения к собранию.</span><span class="sxs-lookup"><span data-stu-id="f8746-115">This is a URL that clients will launch into a browser and will redirect the user to join the meeting.</span></span>|
|<span data-ttu-id="f8746-116">phones</span><span class="sxs-lookup"><span data-stu-id="f8746-116">phones</span></span>|<span data-ttu-id="f8746-117">Коллекция [phone](phone.md)</span><span class="sxs-lookup"><span data-stu-id="f8746-117">[phone](phone.md) collection</span></span>| <span data-ttu-id="f8746-118">Все номера телефонов, связанные с этой Конференции.</span><span class="sxs-lookup"><span data-stu-id="f8746-118">All of the phone numbers associated with this conference.</span></span>|
|<span data-ttu-id="f8746-119">куиккдиал</span><span class="sxs-lookup"><span data-stu-id="f8746-119">quickDial</span></span>|<span data-ttu-id="f8746-120">String</span><span class="sxs-lookup"><span data-stu-id="f8746-120">String</span></span>| <span data-ttu-id="f8746-121">Предварительно отформатированный куиккдиал для этого вызова.</span><span class="sxs-lookup"><span data-stu-id="f8746-121">The pre-formatted quickdial for this call.</span></span>|
|<span data-ttu-id="f8746-122">толлфринумберс</span><span class="sxs-lookup"><span data-stu-id="f8746-122">tollFreeNumbers</span></span>|<span data-ttu-id="f8746-123">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="f8746-123">String collection</span></span>| <span data-ttu-id="f8746-124">Бесплатных бесплатных номеров, которые можно использовать для присоединения к Конференции.</span><span class="sxs-lookup"><span data-stu-id="f8746-124">The toll free numbers that can be used to join the conference.</span></span>|
|<span data-ttu-id="f8746-125">толлнумбер</span><span class="sxs-lookup"><span data-stu-id="f8746-125">tollNumber</span></span>|<span data-ttu-id="f8746-126">String</span><span class="sxs-lookup"><span data-stu-id="f8746-126">String</span></span>| <span data-ttu-id="f8746-127">Платный номер, который можно использовать для присоединения к Конференции.</span><span class="sxs-lookup"><span data-stu-id="f8746-127">The toll number that can be used to join the conference.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f8746-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f8746-128">JSON representation</span></span>

<span data-ttu-id="f8746-129">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f8746-129">The following is a JSON representation of the resource.</span></span>

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
}-->
