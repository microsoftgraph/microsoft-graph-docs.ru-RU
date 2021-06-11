---
title: тип ресурса outOfOfficeSettings
description: Представляет сведения о доступе к телефону для собрания в Интернете.
author: mkhribech
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 13f826babea1e6f9448d1ecb9b8100baaf962b20
ms.sourcegitcommit: 7abb0672a38a6d9b11a2e0d2cc221222cb8358bb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2021
ms.locfileid: "52896636"
---
# <a name="outofofficesettings-resource-type"></a><span data-ttu-id="72b2e-103">тип ресурса outOfOfficeSettings</span><span class="sxs-lookup"><span data-stu-id="72b2e-103">outOfOfficeSettings resource type</span></span>

<span data-ttu-id="72b2e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="72b2e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="72b2e-105">Представляет параметры из офиса, связанные с [присутствием](presence.md) пользователя.</span><span class="sxs-lookup"><span data-stu-id="72b2e-105">Represents the out of office settings related to the [presence](presence.md) of a user.</span></span>

## <a name="properties"></a><span data-ttu-id="72b2e-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="72b2e-106">Properties</span></span>

| <span data-ttu-id="72b2e-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="72b2e-107">Property</span></span>            | <span data-ttu-id="72b2e-108">Тип</span><span class="sxs-lookup"><span data-stu-id="72b2e-108">Type</span></span>    | <span data-ttu-id="72b2e-109">Описание</span><span class="sxs-lookup"><span data-stu-id="72b2e-109">Description</span></span>                                                                    |
|:--------------------|:--------|:-------------------------------------------------------------------------------|
| <span data-ttu-id="72b2e-110">message</span><span class="sxs-lookup"><span data-stu-id="72b2e-110">message</span></span>           | <span data-ttu-id="72b2e-111">String</span><span class="sxs-lookup"><span data-stu-id="72b2e-111">String</span></span>  | <span data-ttu-id="72b2e-112">Неявное сообщение, настроенное пользователем на Outlook клиенте (Автоматические ответы (вне Office)) или клиенте Teams (Расписание вне офиса).</span><span class="sxs-lookup"><span data-stu-id="72b2e-112">The out of office message that the user configured on Outlook client (Automatic Replies (Out of Office)) or the Teams client (Schedule out of office).</span></span> |
| <span data-ttu-id="72b2e-113">isOutOfOffice</span><span class="sxs-lookup"><span data-stu-id="72b2e-113">isOutOfOffice</span></span>      | <span data-ttu-id="72b2e-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="72b2e-114">Boolean</span></span>  | <span data-ttu-id="72b2e-115">True, если либо:</span><span class="sxs-lookup"><span data-stu-id="72b2e-115">True if either:</span></span></br><ul><li><span data-ttu-id="72b2e-116">В настоящее время он находится в неявном окне времени, настроенном на Outlook или Teams клиенте.</span><span class="sxs-lookup"><span data-stu-id="72b2e-116">It is currently in the out of office time window configured on the Outlook or Teams client.</span></span></li><li><span data-ttu-id="72b2e-117">В настоящее время в календаре пользователя имеется событие, помеченное как Show as Out of Office</span><span class="sxs-lookup"><span data-stu-id="72b2e-117">There is currently an event on the user's calendar that's marked as Show as Out of Office</span></span></li></ul></br><span data-ttu-id="72b2e-118">В противном случае, false.</span><span class="sxs-lookup"><span data-stu-id="72b2e-118">Otherwise, false.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="72b2e-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="72b2e-119">JSON representation</span></span>

<span data-ttu-id="72b2e-120">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="72b2e-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.outOfOfficeSettings"
}-->
```json
{
  "message": "String",
  "isOutOfOffice": "Boolean"
}
```
