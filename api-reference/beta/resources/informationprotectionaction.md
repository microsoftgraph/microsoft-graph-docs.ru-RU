---
title: Тип ресурса Информатионпротектионактион
description: Описывает объект абтракт Информатионпротектионактион.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: e8c74bdf5d7199f9ddd1ccba32581c57c30c2713
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42496091"
---
# <a name="informationprotectionaction-resource-type"></a><span data-ttu-id="4fa8d-103">Тип ресурса Информатионпротектионактион</span><span class="sxs-lookup"><span data-stu-id="4fa8d-103">informationProtectionAction resource type</span></span>

<span data-ttu-id="4fa8d-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="4fa8d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4fa8d-105">**Информатионпротектионактион** — это абстрактная сущность, которая возвращается в результате использования любой из API для оценки защиты информации.</span><span class="sxs-lookup"><span data-stu-id="4fa8d-105">The **informationProtectionAction** is an abstract entity that is returned as the result of any of the information protection evaluation APIs.</span></span> <span data-ttu-id="4fa8d-106">Объект содержит одно или несколько из следующих действий, которые указывают приложению, как применять, обновлять или удалять метку защиты информации.</span><span class="sxs-lookup"><span data-stu-id="4fa8d-106">The object contains one or more of the following actions that instruct the application on how to apply, update, or remove the information protection label.</span></span> 

* [<span data-ttu-id="4fa8d-107">аддконтентфутерактион</span><span class="sxs-lookup"><span data-stu-id="4fa8d-107">addContentFooterAction</span></span>](../resources/addcontentfooteraction.md)
* [<span data-ttu-id="4fa8d-108">аддконтенсеадерактион</span><span class="sxs-lookup"><span data-stu-id="4fa8d-108">addContentHeaderAction</span></span>](../resources/addcontentheaderaction.md)
* [<span data-ttu-id="4fa8d-109">аддватермаркактион</span><span class="sxs-lookup"><span data-stu-id="4fa8d-109">addWatermarkAction</span></span>](../resources/addwatermarkaction.md)
* [<span data-ttu-id="4fa8d-110">апплилабелактион</span><span class="sxs-lookup"><span data-stu-id="4fa8d-110">applyLabelAction</span></span>](../resources/applylabelaction.md)
* [<span data-ttu-id="4fa8d-111">Запис</span><span class="sxs-lookup"><span data-stu-id="4fa8d-111">customAction</span></span>](../resources/customaction.md)
* [<span data-ttu-id="4fa8d-112">жустифяктион</span><span class="sxs-lookup"><span data-stu-id="4fa8d-112">justifyAction</span></span>](../resources/justifyaction.md)
* [<span data-ttu-id="4fa8d-113">метадатаактион</span><span class="sxs-lookup"><span data-stu-id="4fa8d-113">metadataAction</span></span>](../resources/metadataaction.md)
* [<span data-ttu-id="4fa8d-114">протектадхокактион</span><span class="sxs-lookup"><span data-stu-id="4fa8d-114">protectAdhocAction</span></span>](../resources/protectadhocaction.md)
* [<span data-ttu-id="4fa8d-115">протектбитемплатеактион</span><span class="sxs-lookup"><span data-stu-id="4fa8d-115">protectByTemplateAction</span></span>](../resources/protectbytemplateaction.md)
* [<span data-ttu-id="4fa8d-116">протектиондонотфорвардактион</span><span class="sxs-lookup"><span data-stu-id="4fa8d-116">protectionDoNotForwardAction</span></span>](../resources/protectdonotforwardaction.md)
* [<span data-ttu-id="4fa8d-117">рекоммендлабелактион</span><span class="sxs-lookup"><span data-stu-id="4fa8d-117">recommendLabelAction</span></span>](../resources/recommendlabelaction.md)
* [<span data-ttu-id="4fa8d-118">ремовеконтентфутерактион</span><span class="sxs-lookup"><span data-stu-id="4fa8d-118">removeContentFooterAction</span></span>](../resources/removecontentfooteraction.md)
* [<span data-ttu-id="4fa8d-119">ремовеконтенсеадерактион</span><span class="sxs-lookup"><span data-stu-id="4fa8d-119">removeContentHeaderAction</span></span>](../resources/removecontentheaderaction.md)
* [<span data-ttu-id="4fa8d-120">ремовепротектионактион</span><span class="sxs-lookup"><span data-stu-id="4fa8d-120">removeProtectionAction</span></span>](../resources/removeprotectionaction.md)
* [<span data-ttu-id="4fa8d-121">ремовеватермаркактион</span><span class="sxs-lookup"><span data-stu-id="4fa8d-121">removeWatermarkAction</span></span>](../resources/removewatermarkaction.md)

## <a name="properties"></a><span data-ttu-id="4fa8d-122">Свойства</span><span class="sxs-lookup"><span data-stu-id="4fa8d-122">Properties</span></span>

<span data-ttu-id="4fa8d-123">Нет</span><span class="sxs-lookup"><span data-stu-id="4fa8d-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4fa8d-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4fa8d-124">JSON representation</span></span>

<span data-ttu-id="4fa8d-125">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4fa8d-125">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.informationProtectionAction",
  "baseType": null
}-->

```json
{

}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "informationProtectionAction resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->