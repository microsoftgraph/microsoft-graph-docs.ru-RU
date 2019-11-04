---
title: Тип ресурса Онлинемитингинфо
description: Сведения для участников, присоединяющихся к собранию в Интернете.
localization_priority: Normal
author: VinodRavichandran
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 7ed8543be8b1d22c797d0033dcd0d41ba6308888
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939392"
---
# <a name="onlinemeetinginfo-resource-type"></a><span data-ttu-id="29e3c-103">Тип ресурса Онлинемитингинфо</span><span class="sxs-lookup"><span data-stu-id="29e3c-103">onlineMeetingInfo resource type</span></span>

<span data-ttu-id="29e3c-104">Сведения для участников, присоединяющихся к собранию в Интернете.</span><span class="sxs-lookup"><span data-stu-id="29e3c-104">Details for an attendee to join the meeting online.</span></span>

## <a name="properties"></a><span data-ttu-id="29e3c-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="29e3c-105">Properties</span></span>

| <span data-ttu-id="29e3c-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="29e3c-106">Property</span></span>     | <span data-ttu-id="29e3c-107">Тип</span><span class="sxs-lookup"><span data-stu-id="29e3c-107">Type</span></span>        | <span data-ttu-id="29e3c-108">Описание</span><span class="sxs-lookup"><span data-stu-id="29e3c-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="29e3c-109">конференцеид</span><span class="sxs-lookup"><span data-stu-id="29e3c-109">conferenceId</span></span>|<span data-ttu-id="29e3c-110">Строка</span><span class="sxs-lookup"><span data-stu-id="29e3c-110">String</span></span>| <span data-ttu-id="29e3c-111">Идентификатор конференции.</span><span class="sxs-lookup"><span data-stu-id="29e3c-111">The ID of the conference.</span></span>|
|<span data-ttu-id="29e3c-112">жоинурл</span><span class="sxs-lookup"><span data-stu-id="29e3c-112">joinUrl</span></span>|<span data-ttu-id="29e3c-113">Строка</span><span class="sxs-lookup"><span data-stu-id="29e3c-113">String</span></span>| <span data-ttu-id="29e3c-114">Внешняя ссылка, которая запускает собрание по сети.</span><span class="sxs-lookup"><span data-stu-id="29e3c-114">The external link that launches the online meeting.</span></span> <span data-ttu-id="29e3c-115">Это URL-адрес, который клиенты будут запускать в браузере и перенаправит пользователя для присоединения к собранию.</span><span class="sxs-lookup"><span data-stu-id="29e3c-115">This is a URL that clients will launch into a browser and will redirect the user to join the meeting.</span></span>|
|<span data-ttu-id="29e3c-116">phones</span><span class="sxs-lookup"><span data-stu-id="29e3c-116">phones</span></span>|<span data-ttu-id="29e3c-117">Коллекция [phone](phone.md)</span><span class="sxs-lookup"><span data-stu-id="29e3c-117">[phone](phone.md) collection</span></span>| <span data-ttu-id="29e3c-118">Все номера телефонов, связанные с этой Конференции.</span><span class="sxs-lookup"><span data-stu-id="29e3c-118">All of the phone numbers associated with this conference.</span></span>|
|<span data-ttu-id="29e3c-119">куиккдиал</span><span class="sxs-lookup"><span data-stu-id="29e3c-119">quickDial</span></span>|<span data-ttu-id="29e3c-120">Строка</span><span class="sxs-lookup"><span data-stu-id="29e3c-120">String</span></span>| <span data-ttu-id="29e3c-121">Предварительно отформатированный куиккдиал для этого вызова.</span><span class="sxs-lookup"><span data-stu-id="29e3c-121">The pre-formatted quickdial for this call.</span></span>|
|<span data-ttu-id="29e3c-122">толлфринумберс</span><span class="sxs-lookup"><span data-stu-id="29e3c-122">tollFreeNumbers</span></span>|<span data-ttu-id="29e3c-123">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="29e3c-123">String collection</span></span>| <span data-ttu-id="29e3c-124">Бесплатных бесплатных номеров, которые можно использовать для присоединения к Конференции.</span><span class="sxs-lookup"><span data-stu-id="29e3c-124">The toll free numbers that can be used to join the conference.</span></span>|
|<span data-ttu-id="29e3c-125">толлнумбер</span><span class="sxs-lookup"><span data-stu-id="29e3c-125">tollNumber</span></span>|<span data-ttu-id="29e3c-126">Строка</span><span class="sxs-lookup"><span data-stu-id="29e3c-126">String</span></span>| <span data-ttu-id="29e3c-127">Платный номер, который можно использовать для присоединения к Конференции.</span><span class="sxs-lookup"><span data-stu-id="29e3c-127">The toll number that can be used to join the conference.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="29e3c-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="29e3c-128">JSON representation</span></span>

<span data-ttu-id="29e3c-129">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="29e3c-129">The following is a JSON representation of the resource.</span></span>

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
