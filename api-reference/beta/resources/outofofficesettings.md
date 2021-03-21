---
title: тип ресурса outOfOfficeSettings
description: Представляет сведения о доступе к телефону для собрания в Интернете.
author: jsandoval-msft
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 018852150ef833d8cb114892790f911b4aad8fe0
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50960384"
---
# <a name="outofofficesettings-resource-type"></a><span data-ttu-id="9f508-103">тип ресурса outOfOfficeSettings</span><span class="sxs-lookup"><span data-stu-id="9f508-103">outOfOfficeSettings resource type</span></span>

<span data-ttu-id="9f508-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9f508-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9f508-105">Представляет параметры из офиса, связанные с [присутствием](presence.md) пользователя.</span><span class="sxs-lookup"><span data-stu-id="9f508-105">Represents the out of office settings related to the [presence](presence.md) of a user.</span></span>

## <a name="properties"></a><span data-ttu-id="9f508-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="9f508-106">Properties</span></span>

| <span data-ttu-id="9f508-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="9f508-107">Property</span></span>            | <span data-ttu-id="9f508-108">Тип</span><span class="sxs-lookup"><span data-stu-id="9f508-108">Type</span></span>    | <span data-ttu-id="9f508-109">Описание</span><span class="sxs-lookup"><span data-stu-id="9f508-109">Description</span></span>                                                                    |
|:--------------------|:--------|:-------------------------------------------------------------------------------|
| <span data-ttu-id="9f508-110">message</span><span class="sxs-lookup"><span data-stu-id="9f508-110">message</span></span>           | <span data-ttu-id="9f508-111">String</span><span class="sxs-lookup"><span data-stu-id="9f508-111">String</span></span>  | <span data-ttu-id="9f508-112">Сообщение из офиса, настроенное пользователем в клиенте Outlook (Автоматические ответы (вне Office)) или клиенте Teams (Расписание вне офиса).</span><span class="sxs-lookup"><span data-stu-id="9f508-112">The out of office message that the user configured on Outlook client (Automatic Replies (Out of Office)) or the Teams client (Schedule out of office).</span></span> |
| <span data-ttu-id="9f508-113">isOutOfOffice</span><span class="sxs-lookup"><span data-stu-id="9f508-113">isOutOfOffice</span></span>      | <span data-ttu-id="9f508-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f508-114">Boolean</span></span>  | <span data-ttu-id="9f508-115">True, если либо:</span><span class="sxs-lookup"><span data-stu-id="9f508-115">True if either:</span></span></br><ul><li><span data-ttu-id="9f508-116">В настоящее время он находится в окне вне офиса, настроенном на клиент Outlook или Teams.</span><span class="sxs-lookup"><span data-stu-id="9f508-116">It is currently in the out of office time window configured on the Outlook or Teams client.</span></span></li><li><span data-ttu-id="9f508-117">В настоящее время в календаре пользователя имеется событие, помеченное как Show as Out of Office</span><span class="sxs-lookup"><span data-stu-id="9f508-117">There is currently an event on the user's calendar that's marked as Show as Out of Office</span></span></li></ul></br><span data-ttu-id="9f508-118">В противном случае, false.</span><span class="sxs-lookup"><span data-stu-id="9f508-118">Otherwise, false.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="9f508-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9f508-119">JSON representation</span></span>

<span data-ttu-id="9f508-120">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9f508-120">The following is a JSON representation of the resource.</span></span>

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
