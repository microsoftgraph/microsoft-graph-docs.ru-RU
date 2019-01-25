---
title: Тип ресурса educationSynchronizationError
description: Представляет ошибку во время проверки данных профиля school и/или синхронизации. Уникальный ошибка создается для каждой записи, не удается проверить и/или синхронизация с Azure Active Directory (Azure AD).
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 5c937e95441132e4633b0f5e48a75b0597b8f08d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525145"
---
# <a name="educationsynchronizationerror-resource-type"></a><span data-ttu-id="061da-103">Тип ресурса educationSynchronizationError</span><span class="sxs-lookup"><span data-stu-id="061da-103">educationSynchronizationError resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="061da-104">Представляет ошибку во время проверки данных профиля school и/или синхронизации. Уникальный ошибка создается для каждой записи, не удается проверить и/или синхронизация с Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="061da-104">Represents an error during school data profile validation and/or sync. A unique error is generated for every entry that fails to validate and/or synchronize with Azure Active Directory (Azure AD).</span></span>

## <a name="methods"></a><span data-ttu-id="061da-105">Методы</span><span class="sxs-lookup"><span data-stu-id="061da-105">Methods</span></span>

| <span data-ttu-id="061da-106">Метод</span><span class="sxs-lookup"><span data-stu-id="061da-106">Method</span></span> | <span data-ttu-id="061da-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="061da-107">Return Type</span></span> | <span data-ttu-id="061da-108">Описание</span><span class="sxs-lookup"><span data-stu-id="061da-108">Description</span></span> |
|:-|:-|:-|
| [<span data-ttu-id="061da-109">Получение ошибки синхронизации</span><span class="sxs-lookup"><span data-stu-id="061da-109">Get synchronization errors</span></span>](../api/educationsynchronizationerrors-get.md) | <span data-ttu-id="061da-110">**educationSynchronizationError** коллекции</span><span class="sxs-lookup"><span data-stu-id="061da-110">**educationSynchronizationError** collection</span></span>| <span data-ttu-id="061da-111">Возвращает список ошибок синхронизации службы, связанные с профилем.</span><span class="sxs-lookup"><span data-stu-id="061da-111">Returns the list of synchronization errors associated with a profile.</span></span> |

## <a name="properties"></a><span data-ttu-id="061da-112">Свойства</span><span class="sxs-lookup"><span data-stu-id="061da-112">Properties</span></span>

| <span data-ttu-id="061da-113">Свойство</span><span class="sxs-lookup"><span data-stu-id="061da-113">Property</span></span> | <span data-ttu-id="061da-114">Тип</span><span class="sxs-lookup"><span data-stu-id="061da-114">Type</span></span> | <span data-ttu-id="061da-115">Описание</span><span class="sxs-lookup"><span data-stu-id="061da-115">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="061da-116">**entryType**</span><span class="sxs-lookup"><span data-stu-id="061da-116">**entryType**</span></span> | <span data-ttu-id="061da-117">string</span><span class="sxs-lookup"><span data-stu-id="061da-117">string</span></span> |  <span data-ttu-id="061da-118">Представляет сущности синхронизации (школа, раздел, учебы, преподаватель).</span><span class="sxs-lookup"><span data-stu-id="061da-118">Represents the sync entity (school, section, student, teacher).</span></span>       |
| <span data-ttu-id="061da-119">errorCode</span><span class="sxs-lookup"><span data-stu-id="061da-119">**errorCode**</span></span> | <span data-ttu-id="061da-120">string</span><span class="sxs-lookup"><span data-stu-id="061da-120">string</span></span> |  <span data-ttu-id="061da-121">Представляет код ошибки для этой ошибки.</span><span class="sxs-lookup"><span data-stu-id="061da-121">Represents the error code for this error.</span></span>         |
| <span data-ttu-id="061da-122">**ErrorMessage**</span><span class="sxs-lookup"><span data-stu-id="061da-122">**errorMessage**</span></span> | <span data-ttu-id="061da-123">string</span><span class="sxs-lookup"><span data-stu-id="061da-123">string</span></span> |  <span data-ttu-id="061da-124">Содержит описание ошибки.</span><span class="sxs-lookup"><span data-stu-id="061da-124">Contains a description of the error.</span></span>        |
| <span data-ttu-id="061da-125">**joiningValue**</span><span class="sxs-lookup"><span data-stu-id="061da-125">**joiningValue**</span></span> | <span data-ttu-id="061da-126">string</span><span class="sxs-lookup"><span data-stu-id="061da-126">string</span></span> |  <span data-ttu-id="061da-127">Уникальный идентификатор для записи.</span><span class="sxs-lookup"><span data-stu-id="061da-127">The unique identifier for the entry.</span></span>         |
| <span data-ttu-id="061da-128">recordedDateTime</span><span class="sxs-lookup"><span data-stu-id="061da-128">**recordedDateTime**</span></span> | <span data-ttu-id="061da-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="061da-129">DateTimeOffset</span></span> | <span data-ttu-id="061da-130">Время возникновения этой ошибки.</span><span class="sxs-lookup"><span data-stu-id="061da-130">The time of occurrence of this error.</span></span>         |
| <span data-ttu-id="061da-131">**reportableIdentifier**</span><span class="sxs-lookup"><span data-stu-id="061da-131">**reportableIdentifier**</span></span> | <span data-ttu-id="061da-132">string</span><span class="sxs-lookup"><span data-stu-id="061da-132">string</span></span> | <span data-ttu-id="061da-133">Идентификатор элемента в этой записи об ошибках.</span><span class="sxs-lookup"><span data-stu-id="061da-133">The identifier of this error entry.</span></span>       |

## <a name="json-representation"></a><span data-ttu-id="061da-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="061da-134">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSynchronizationError"
}-->

```json
{
    "entryType": "String",
    "errorCode": "String",
    "errorMessage": "String",
    "joiningValue": "String",
    "recordedDateTime": "DateTimeOffset",
    "reportableIdentifier": "String"
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationsynchronizationerror.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
