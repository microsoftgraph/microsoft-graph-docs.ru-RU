---
title: пендингконтентупдате
description: Ресурс Пендингконтентупдате указывает на то, что операция, которая может повлиять на двоичный контент driveItem, ожидает завершения.
localization_priority: Normal
author: learafa
ms.prod: files
doc_type: resourcePageType
ms.openlocfilehash: b1a197ae60dc8bb60533d567c6472a65988c3962
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: Auto
ms.contentlocale: ru-RU
ms.lasthandoff: 06/24/2020
ms.locfileid: "44863805"
---
# <a name="pendingcontentupdate-resource-type"></a><span data-ttu-id="702fa-103">Тип ресурса Пендингконтентупдате</span><span class="sxs-lookup"><span data-stu-id="702fa-103">pendingContentUpdate resource type</span></span>

<span data-ttu-id="702fa-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="702fa-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="702fa-105">Указывает, что операция, которая может повлиять на двоичное содержимое **driveItem** , ожидает завершения.</span><span class="sxs-lookup"><span data-stu-id="702fa-105">Indicates that an operation that might affect the binary content of the **driveItem** is pending completion.</span></span>

## <a name="properties"></a><span data-ttu-id="702fa-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="702fa-106">Properties</span></span>

| <span data-ttu-id="702fa-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="702fa-107">Property</span></span>     | <span data-ttu-id="702fa-108">Тип</span><span class="sxs-lookup"><span data-stu-id="702fa-108">Type</span></span>         | <span data-ttu-id="702fa-109">Описание</span><span class="sxs-lookup"><span data-stu-id="702fa-109">Description</span></span> |
|:-------------|:-------------|:------------|
|<span data-ttu-id="702fa-110">**куеуеддатетиме**</span><span class="sxs-lookup"><span data-stu-id="702fa-110">**queuedDateTime**</span></span>|<span data-ttu-id="702fa-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="702fa-111">DateTimeOffset</span></span>|<span data-ttu-id="702fa-112">Дата и время, когда отложенная двоичная операция была поставлена в очередь в течение времени в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="702fa-112">Date and time the pending binary operation was queued in UTC time.</span></span> <span data-ttu-id="702fa-113">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="702fa-113">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="702fa-114">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="702fa-114">JSON representation</span></span>

<span data-ttu-id="702fa-115">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="702fa-115">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.pendingContentUpdate",
  "baseType": null
}-->

```json
{
  "queuedDateTime": "String (timestamp)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "The pendingContentUpdate resource indicates that an operation that may affect the binary content of the DriveItem is pending completion.",
  "keywords": "pendingoperation,operation,pendingcontentupdate",
  "section": "documentation",
  "tocPath": ""
}-->
