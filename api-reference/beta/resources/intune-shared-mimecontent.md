---
title: Тип ресурса mimeContent
description: Содержит свойства обычного содержимого MIME.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ee38eee9100982f6dc5f22315af480a783cc4252
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27962123"
---
# <a name="mimecontent-resource-type"></a><span data-ttu-id="65c31-103">Тип ресурса mimeContent</span><span class="sxs-lookup"><span data-stu-id="65c31-103">mimeContent resource type</span></span>

> <span data-ttu-id="65c31-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="65c31-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="65c31-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="65c31-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="65c31-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="65c31-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="65c31-107">Содержит свойства обычного содержимого MIME.</span><span class="sxs-lookup"><span data-stu-id="65c31-107">Contains properties for a generic mime content.</span></span>
## <a name="properties"></a><span data-ttu-id="65c31-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="65c31-108">Properties</span></span>
|<span data-ttu-id="65c31-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="65c31-109">Property</span></span>|<span data-ttu-id="65c31-110">Тип</span><span class="sxs-lookup"><span data-stu-id="65c31-110">Type</span></span>|<span data-ttu-id="65c31-111">Описание</span><span class="sxs-lookup"><span data-stu-id="65c31-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="65c31-112">type</span><span class="sxs-lookup"><span data-stu-id="65c31-112">type</span></span>|<span data-ttu-id="65c31-113">Строка</span><span class="sxs-lookup"><span data-stu-id="65c31-113">String</span></span>|<span data-ttu-id="65c31-114">Указывает MIME-тип содержимого.</span><span class="sxs-lookup"><span data-stu-id="65c31-114">Indicates the content mime type.</span></span>|
|<span data-ttu-id="65c31-115">value</span><span class="sxs-lookup"><span data-stu-id="65c31-115">value</span></span>|<span data-ttu-id="65c31-116">Binary</span><span class="sxs-lookup"><span data-stu-id="65c31-116">Binary</span></span>|<span data-ttu-id="65c31-117">Массив байтов содержимого.</span><span class="sxs-lookup"><span data-stu-id="65c31-117">The byte array that contains the actual content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="65c31-118">Связи</span><span class="sxs-lookup"><span data-stu-id="65c31-118">Relationships</span></span>
<span data-ttu-id="65c31-119">Нет</span><span class="sxs-lookup"><span data-stu-id="65c31-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="65c31-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="65c31-120">JSON Representation</span></span>
<span data-ttu-id="65c31-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="65c31-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mimeContent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mimeContent",
  "type": "String",
  "value": "binary"
}
```





