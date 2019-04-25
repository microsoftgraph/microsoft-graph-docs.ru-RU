---
title: Тип ресурса educationSynchronizationError
description: Представляет ошибку во время проверки и/или синхронизации профиля данных учебного заведения. Для каждой записи, которая не проходит проверку и/или синхронизируется с помощью Azure Active Directory (Azure AD), создается уникальная ошибка.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 5c937e95441132e4633b0f5e48a75b0597b8f08d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32542968"
---
# <a name="educationsynchronizationerror-resource-type"></a><span data-ttu-id="d5e37-103">Тип ресурса educationSynchronizationError</span><span class="sxs-lookup"><span data-stu-id="d5e37-103">educationSynchronizationError resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d5e37-104">Представляет ошибку во время проверки и/или синхронизации профиля данных учебного заведения. Для каждой записи, которая не проходит проверку и/или синхронизируется с помощью Azure Active Directory (Azure AD), создается уникальная ошибка.</span><span class="sxs-lookup"><span data-stu-id="d5e37-104">Represents an error during school data profile validation and/or sync. A unique error is generated for every entry that fails to validate and/or synchronize with Azure Active Directory (Azure AD).</span></span>

## <a name="methods"></a><span data-ttu-id="d5e37-105">Методы</span><span class="sxs-lookup"><span data-stu-id="d5e37-105">Methods</span></span>

| <span data-ttu-id="d5e37-106">Метод</span><span class="sxs-lookup"><span data-stu-id="d5e37-106">Method</span></span> | <span data-ttu-id="d5e37-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="d5e37-107">Return Type</span></span> | <span data-ttu-id="d5e37-108">Описание</span><span class="sxs-lookup"><span data-stu-id="d5e37-108">Description</span></span> |
|:-|:-|:-|
| [<span data-ttu-id="d5e37-109">Получение ошибок синхронизации</span><span class="sxs-lookup"><span data-stu-id="d5e37-109">Get synchronization errors</span></span>](../api/educationsynchronizationerrors-get.md) | <span data-ttu-id="d5e37-110">Коллекция **educationSynchronizationError**</span><span class="sxs-lookup"><span data-stu-id="d5e37-110">**educationSynchronizationError** collection</span></span>| <span data-ttu-id="d5e37-111">Возвращает список ошибок синхронизации, связанных с профилем.</span><span class="sxs-lookup"><span data-stu-id="d5e37-111">Returns the list of synchronization errors associated with a profile.</span></span> |

## <a name="properties"></a><span data-ttu-id="d5e37-112">Свойства</span><span class="sxs-lookup"><span data-stu-id="d5e37-112">Properties</span></span>

| <span data-ttu-id="d5e37-113">Свойство</span><span class="sxs-lookup"><span data-stu-id="d5e37-113">Property</span></span> | <span data-ttu-id="d5e37-114">Тип</span><span class="sxs-lookup"><span data-stu-id="d5e37-114">Type</span></span> | <span data-ttu-id="d5e37-115">Описание</span><span class="sxs-lookup"><span data-stu-id="d5e37-115">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="d5e37-116">**Ентритипе**</span><span class="sxs-lookup"><span data-stu-id="d5e37-116">**entryType**</span></span> | <span data-ttu-id="d5e37-117">string</span><span class="sxs-lookup"><span data-stu-id="d5e37-117">string</span></span> |  <span data-ttu-id="d5e37-118">Представляет объект синхронизации (School, section, Student, преподаватель).</span><span class="sxs-lookup"><span data-stu-id="d5e37-118">Represents the sync entity (school, section, student, teacher).</span></span>       |
| <span data-ttu-id="d5e37-119">**Коде**</span><span class="sxs-lookup"><span data-stu-id="d5e37-119">**errorCode**</span></span> | <span data-ttu-id="d5e37-120">string</span><span class="sxs-lookup"><span data-stu-id="d5e37-120">string</span></span> |  <span data-ttu-id="d5e37-121">Представляет код ошибки для этой ошибки.</span><span class="sxs-lookup"><span data-stu-id="d5e37-121">Represents the error code for this error.</span></span>         |
| <span data-ttu-id="d5e37-122">**Ошибк**</span><span class="sxs-lookup"><span data-stu-id="d5e37-122">**errorMessage**</span></span> | <span data-ttu-id="d5e37-123">string</span><span class="sxs-lookup"><span data-stu-id="d5e37-123">string</span></span> |  <span data-ttu-id="d5e37-124">Содержит описание ошибки.</span><span class="sxs-lookup"><span data-stu-id="d5e37-124">Contains a description of the error.</span></span>        |
| <span data-ttu-id="d5e37-125">**Жоинингвалуе**</span><span class="sxs-lookup"><span data-stu-id="d5e37-125">**joiningValue**</span></span> | <span data-ttu-id="d5e37-126">string</span><span class="sxs-lookup"><span data-stu-id="d5e37-126">string</span></span> |  <span data-ttu-id="d5e37-127">Уникальный идентификатор для записи.</span><span class="sxs-lookup"><span data-stu-id="d5e37-127">The unique identifier for the entry.</span></span>         |
| <span data-ttu-id="d5e37-128">**recordedDateTime**</span><span class="sxs-lookup"><span data-stu-id="d5e37-128">**recordedDateTime**</span></span> | <span data-ttu-id="d5e37-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d5e37-129">DateTimeOffset</span></span> | <span data-ttu-id="d5e37-130">Время возникновения ошибки.</span><span class="sxs-lookup"><span data-stu-id="d5e37-130">The time of occurrence of this error.</span></span>         |
| <span data-ttu-id="d5e37-131">**Репортаблеидентифиер**</span><span class="sxs-lookup"><span data-stu-id="d5e37-131">**reportableIdentifier**</span></span> | <span data-ttu-id="d5e37-132">string</span><span class="sxs-lookup"><span data-stu-id="d5e37-132">string</span></span> | <span data-ttu-id="d5e37-133">Идентификатор этой записи об ошибке.</span><span class="sxs-lookup"><span data-stu-id="d5e37-133">The identifier of this error entry.</span></span>       |

## <a name="json-representation"></a><span data-ttu-id="d5e37-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d5e37-134">JSON representation</span></span>
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
