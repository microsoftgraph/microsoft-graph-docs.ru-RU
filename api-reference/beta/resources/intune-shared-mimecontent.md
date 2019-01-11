---
title: Тип ресурса mimeContent
description: Содержит свойства обычного содержимого MIME.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 826606d41feb0f0a156a1b8240bde7f4ac926a5a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27838229"
---
# <a name="mimecontent-resource-type"></a><span data-ttu-id="0f042-103">Тип ресурса mimeContent</span><span class="sxs-lookup"><span data-stu-id="0f042-103">mimeContent resource type</span></span>

> <span data-ttu-id="0f042-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="0f042-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0f042-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0f042-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0f042-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="0f042-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0f042-107">Содержит свойства обычного содержимого MIME.</span><span class="sxs-lookup"><span data-stu-id="0f042-107">Contains properties for a generic mime content.</span></span>
## <a name="properties"></a><span data-ttu-id="0f042-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="0f042-108">Properties</span></span>
|<span data-ttu-id="0f042-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="0f042-109">Property</span></span>|<span data-ttu-id="0f042-110">Тип</span><span class="sxs-lookup"><span data-stu-id="0f042-110">Type</span></span>|<span data-ttu-id="0f042-111">Описание</span><span class="sxs-lookup"><span data-stu-id="0f042-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0f042-112">type</span><span class="sxs-lookup"><span data-stu-id="0f042-112">type</span></span>|<span data-ttu-id="0f042-113">Строка</span><span class="sxs-lookup"><span data-stu-id="0f042-113">String</span></span>|<span data-ttu-id="0f042-114">Указывает MIME-тип содержимого.</span><span class="sxs-lookup"><span data-stu-id="0f042-114">Indicates the content mime type.</span></span>|
|<span data-ttu-id="0f042-115">value</span><span class="sxs-lookup"><span data-stu-id="0f042-115">value</span></span>|<span data-ttu-id="0f042-116">Binary</span><span class="sxs-lookup"><span data-stu-id="0f042-116">Binary</span></span>|<span data-ttu-id="0f042-117">Массив байтов содержимого.</span><span class="sxs-lookup"><span data-stu-id="0f042-117">The byte array that contains the actual content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0f042-118">Связи</span><span class="sxs-lookup"><span data-stu-id="0f042-118">Relationships</span></span>
<span data-ttu-id="0f042-119">Нет</span><span class="sxs-lookup"><span data-stu-id="0f042-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="0f042-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0f042-120">JSON Representation</span></span>
<span data-ttu-id="0f042-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0f042-121">Here is a JSON representation of the resource.</span></span>
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





