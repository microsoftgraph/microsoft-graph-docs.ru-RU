---
title: тип ресурса printDocument
description: Представляет печатаемый документ.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: d8ca73a6e8acfb6ac2326b171b2b8c04fed7e039
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517948"
---
# <a name="printdocument-resource-type"></a><span data-ttu-id="39e6b-103">тип ресурса printDocument</span><span class="sxs-lookup"><span data-stu-id="39e6b-103">printDocument resource type</span></span>

<span data-ttu-id="39e6b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="39e6b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="39e6b-105">Представляет печатаемый документ.</span><span class="sxs-lookup"><span data-stu-id="39e6b-105">Represents a document being printed.</span></span>

## <a name="methods"></a><span data-ttu-id="39e6b-106">Методы</span><span class="sxs-lookup"><span data-stu-id="39e6b-106">Methods</span></span>
|<span data-ttu-id="39e6b-107">Метод</span><span class="sxs-lookup"><span data-stu-id="39e6b-107">Method</span></span>|<span data-ttu-id="39e6b-108">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="39e6b-108">Return type</span></span>|<span data-ttu-id="39e6b-109">Описание</span><span class="sxs-lookup"><span data-stu-id="39e6b-109">Description</span></span>|
|:---|:---|:---|
| [<span data-ttu-id="39e6b-110">Создание сеанса загрузки</span><span class="sxs-lookup"><span data-stu-id="39e6b-110">Create upload session</span></span>](../api/printdocument-createuploadsession.md) | [<span data-ttu-id="39e6b-111">uploadSession</span><span class="sxs-lookup"><span data-stu-id="39e6b-111">uploadSession</span></span>](uploadsession.md) | <span data-ttu-id="39e6b-112">Создание сеанса загрузки в итеративный диапазоны загрузки двоичного файла **printDocument**.</span><span class="sxs-lookup"><span data-stu-id="39e6b-112">Create an upload session to iteratively upload ranges of binary file of the **printDocument**.</span></span> |
| [<span data-ttu-id="39e6b-113">Скачивание двоичного файла</span><span class="sxs-lookup"><span data-stu-id="39e6b-113">Download binary file</span></span>](../api/printdocument-get-file.md) | <span data-ttu-id="39e6b-114">Скачать URL-адрес</span><span class="sxs-lookup"><span data-stu-id="39e6b-114">Download Url</span></span> | <span data-ttu-id="39e6b-115">Скачайте двоичный файл, связанный с **печатьюDocument**.</span><span class="sxs-lookup"><span data-stu-id="39e6b-115">Download the binary file associated with the **printDocument**.</span></span> |

## <a name="properties"></a><span data-ttu-id="39e6b-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="39e6b-116">Properties</span></span>
|<span data-ttu-id="39e6b-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="39e6b-117">Property</span></span>|<span data-ttu-id="39e6b-118">Тип</span><span class="sxs-lookup"><span data-stu-id="39e6b-118">Type</span></span>|<span data-ttu-id="39e6b-119">Описание</span><span class="sxs-lookup"><span data-stu-id="39e6b-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="39e6b-120">id</span><span class="sxs-lookup"><span data-stu-id="39e6b-120">id</span></span>|<span data-ttu-id="39e6b-121">Строка</span><span class="sxs-lookup"><span data-stu-id="39e6b-121">String</span></span>|<span data-ttu-id="39e6b-122">Идентификатор документа.</span><span class="sxs-lookup"><span data-stu-id="39e6b-122">The document's identifier.</span></span> <span data-ttu-id="39e6b-123">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="39e6b-123">Read-only.</span></span>|
|<span data-ttu-id="39e6b-124">displayName</span><span class="sxs-lookup"><span data-stu-id="39e6b-124">displayName</span></span>|<span data-ttu-id="39e6b-125">Строка</span><span class="sxs-lookup"><span data-stu-id="39e6b-125">String</span></span>|<span data-ttu-id="39e6b-126">Имя документа.</span><span class="sxs-lookup"><span data-stu-id="39e6b-126">The document's name.</span></span> <span data-ttu-id="39e6b-127">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="39e6b-127">Read-only.</span></span>|
|<span data-ttu-id="39e6b-128">contentType</span><span class="sxs-lookup"><span data-stu-id="39e6b-128">contentType</span></span>|<span data-ttu-id="39e6b-129">String</span><span class="sxs-lookup"><span data-stu-id="39e6b-129">String</span></span>|<span data-ttu-id="39e6b-130">Тип контента документа (MIME).</span><span class="sxs-lookup"><span data-stu-id="39e6b-130">The document's content (MIME) type.</span></span> <span data-ttu-id="39e6b-131">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="39e6b-131">Read-only.</span></span>|
|<span data-ttu-id="39e6b-132">size</span><span class="sxs-lookup"><span data-stu-id="39e6b-132">size</span></span>|<span data-ttu-id="39e6b-133">Int64</span><span class="sxs-lookup"><span data-stu-id="39e6b-133">Int64</span></span>|<span data-ttu-id="39e6b-134">Размер документа в bytes.</span><span class="sxs-lookup"><span data-stu-id="39e6b-134">The document's size in bytes.</span></span> <span data-ttu-id="39e6b-135">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="39e6b-135">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="39e6b-136">Отношения</span><span class="sxs-lookup"><span data-stu-id="39e6b-136">Relationships</span></span>
<span data-ttu-id="39e6b-137">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="39e6b-137">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="39e6b-138">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="39e6b-138">JSON representation</span></span>
<span data-ttu-id="39e6b-139">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="39e6b-139">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.printDocument",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printDocument",
  "id": "String (identifier)",
  "displayName": "String",
  "contentType": "String",
  "size": "Integer"
}
```