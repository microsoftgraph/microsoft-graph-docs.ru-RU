---
title: Тип ресурса outOfOfficeSettings
description: Представляет сведения о доступе по телефону для собрания по сети.
author: elvinyang-msft
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 4e3e179ec752cfffc4ae4711d9fd0bc541f1506d
ms.sourcegitcommit: 6d04db95bf233d6819d24b01fd7f8b6db57a524c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2021
ms.locfileid: "49796783"
---
# <a name="outofofficesettings-resource-type"></a><span data-ttu-id="b2211-103">Тип ресурса outOfOfficeSettings</span><span class="sxs-lookup"><span data-stu-id="b2211-103">outOfOfficeSettings resource type</span></span>

<span data-ttu-id="b2211-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b2211-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b2211-105">Представляет параметры "Нет на месте", связанные с [присутствием](presence.md) пользователя.</span><span class="sxs-lookup"><span data-stu-id="b2211-105">Represents the out of office settings related to the [presence](presence.md) of a user.</span></span>

## <a name="properties"></a><span data-ttu-id="b2211-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="b2211-106">Properties</span></span>

| <span data-ttu-id="b2211-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="b2211-107">Property</span></span>            | <span data-ttu-id="b2211-108">Тип</span><span class="sxs-lookup"><span data-stu-id="b2211-108">Type</span></span>    | <span data-ttu-id="b2211-109">Описание</span><span class="sxs-lookup"><span data-stu-id="b2211-109">Description</span></span>                                                                    |
|:--------------------|:--------|:-------------------------------------------------------------------------------|
| <span data-ttu-id="b2211-110">message</span><span class="sxs-lookup"><span data-stu-id="b2211-110">message</span></span>           | <span data-ttu-id="b2211-111">String</span><span class="sxs-lookup"><span data-stu-id="b2211-111">String</span></span>  | <span data-ttu-id="b2211-112">Сообщение об простое, настроенное пользователем в клиенте Outlook (автоматические ответы (нет на офисе) или клиенте Teams (запланировать выход из офиса).</span><span class="sxs-lookup"><span data-stu-id="b2211-112">The out of office message that the user configured on Outlook client (Automatic Replies (Out of Office)) or the Teams client (Schedule out of office).</span></span> |
| <span data-ttu-id="b2211-113">isOutOfOffice</span><span class="sxs-lookup"><span data-stu-id="b2211-113">isOutOfOffice</span></span>      | <span data-ttu-id="b2211-114">Логический</span><span class="sxs-lookup"><span data-stu-id="b2211-114">Boolean</span></span>  | <span data-ttu-id="b2211-115">True, если один из них:</span><span class="sxs-lookup"><span data-stu-id="b2211-115">True if either:</span></span></br><ul><li><span data-ttu-id="b2211-116">В настоящее время он находится в периоде простоя, настроенного в клиенте Outlook или Teams.</span><span class="sxs-lookup"><span data-stu-id="b2211-116">It is currently in the out of office time window configured on the Outlook or Teams client.</span></span></li><li><span data-ttu-id="b2211-117">В настоящее время в календаре пользователя есть событие, помеченное как "Показать как нет на офисе"</span><span class="sxs-lookup"><span data-stu-id="b2211-117">There is currently an event on the user's calendar that's marked as Show as Out of Office</span></span></li></ul></br><span data-ttu-id="b2211-118">В противном случае false.</span><span class="sxs-lookup"><span data-stu-id="b2211-118">Otherwise, false.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b2211-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b2211-119">JSON representation</span></span>

<span data-ttu-id="b2211-120">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b2211-120">The following is a JSON representation of the resource.</span></span>

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
