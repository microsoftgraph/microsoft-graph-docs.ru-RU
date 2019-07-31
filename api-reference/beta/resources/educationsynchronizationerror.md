---
title: Тип ресурса educationSynchronizationError
description: Представляет ошибку во время проверки и/или синхронизации профиля данных учебного заведения. Для каждой записи, которая не проходит проверку и/или синхронизируется с помощью Azure Active Directory (Azure AD), создается уникальная ошибка.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 11e5be9893c6a50615774e0d2a8e4d51c9576da6
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972413"
---
# <a name="educationsynchronizationerror-resource-type"></a><span data-ttu-id="6920e-103">Тип ресурса educationSynchronizationError</span><span class="sxs-lookup"><span data-stu-id="6920e-103">educationSynchronizationError resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6920e-104">Представляет ошибку во время проверки и/или синхронизации профиля данных учебного заведения. Для каждой записи, которая не проходит проверку и/или синхронизируется с помощью Azure Active Directory (Azure AD), создается уникальная ошибка.</span><span class="sxs-lookup"><span data-stu-id="6920e-104">Represents an error during school data profile validation and/or sync. A unique error is generated for every entry that fails to validate and/or synchronize with Azure Active Directory (Azure AD).</span></span>

## <a name="methods"></a><span data-ttu-id="6920e-105">Методы</span><span class="sxs-lookup"><span data-stu-id="6920e-105">Methods</span></span>

| <span data-ttu-id="6920e-106">Метод</span><span class="sxs-lookup"><span data-stu-id="6920e-106">Method</span></span> | <span data-ttu-id="6920e-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="6920e-107">Return Type</span></span> | <span data-ttu-id="6920e-108">Описание</span><span class="sxs-lookup"><span data-stu-id="6920e-108">Description</span></span> |
|:-|:-|:-|
| [<span data-ttu-id="6920e-109">Получение ошибок синхронизации</span><span class="sxs-lookup"><span data-stu-id="6920e-109">Get synchronization errors</span></span>](../api/educationsynchronizationerrors-get.md) | <span data-ttu-id="6920e-110">Коллекция **educationSynchronizationError**</span><span class="sxs-lookup"><span data-stu-id="6920e-110">**educationSynchronizationError** collection</span></span>| <span data-ttu-id="6920e-111">Возвращает список ошибок синхронизации, связанных с профилем.</span><span class="sxs-lookup"><span data-stu-id="6920e-111">Returns the list of synchronization errors associated with a profile.</span></span> |

## <a name="properties"></a><span data-ttu-id="6920e-112">Свойства</span><span class="sxs-lookup"><span data-stu-id="6920e-112">Properties</span></span>

| <span data-ttu-id="6920e-113">Свойство</span><span class="sxs-lookup"><span data-stu-id="6920e-113">Property</span></span> | <span data-ttu-id="6920e-114">Тип</span><span class="sxs-lookup"><span data-stu-id="6920e-114">Type</span></span> | <span data-ttu-id="6920e-115">Описание</span><span class="sxs-lookup"><span data-stu-id="6920e-115">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="6920e-116">**Ентритипе**</span><span class="sxs-lookup"><span data-stu-id="6920e-116">**entryType**</span></span> | <span data-ttu-id="6920e-117">string</span><span class="sxs-lookup"><span data-stu-id="6920e-117">string</span></span> |  <span data-ttu-id="6920e-118">Представляет объект синхронизации (School, section, Student, преподаватель).</span><span class="sxs-lookup"><span data-stu-id="6920e-118">Represents the sync entity (school, section, student, teacher).</span></span>       |
| <span data-ttu-id="6920e-119">**Коде**</span><span class="sxs-lookup"><span data-stu-id="6920e-119">**errorCode**</span></span> | <span data-ttu-id="6920e-120">string</span><span class="sxs-lookup"><span data-stu-id="6920e-120">string</span></span> |  <span data-ttu-id="6920e-121">Представляет код ошибки для этой ошибки.</span><span class="sxs-lookup"><span data-stu-id="6920e-121">Represents the error code for this error.</span></span>         |
| <span data-ttu-id="6920e-122">**Ошибк**</span><span class="sxs-lookup"><span data-stu-id="6920e-122">**errorMessage**</span></span> | <span data-ttu-id="6920e-123">string</span><span class="sxs-lookup"><span data-stu-id="6920e-123">string</span></span> |  <span data-ttu-id="6920e-124">Содержит описание ошибки.</span><span class="sxs-lookup"><span data-stu-id="6920e-124">Contains a description of the error.</span></span>        |
| <span data-ttu-id="6920e-125">**Жоинингвалуе**</span><span class="sxs-lookup"><span data-stu-id="6920e-125">**joiningValue**</span></span> | <span data-ttu-id="6920e-126">string</span><span class="sxs-lookup"><span data-stu-id="6920e-126">string</span></span> |  <span data-ttu-id="6920e-127">Уникальный идентификатор для записи.</span><span class="sxs-lookup"><span data-stu-id="6920e-127">The unique identifier for the entry.</span></span>         |
| <span data-ttu-id="6920e-128">**recordedDateTime**</span><span class="sxs-lookup"><span data-stu-id="6920e-128">**recordedDateTime**</span></span> | <span data-ttu-id="6920e-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6920e-129">DateTimeOffset</span></span> | <span data-ttu-id="6920e-130">Время возникновения ошибки.</span><span class="sxs-lookup"><span data-stu-id="6920e-130">The time of occurrence of this error.</span></span>         |
| <span data-ttu-id="6920e-131">**Репортаблеидентифиер**</span><span class="sxs-lookup"><span data-stu-id="6920e-131">**reportableIdentifier**</span></span> | <span data-ttu-id="6920e-132">string</span><span class="sxs-lookup"><span data-stu-id="6920e-132">string</span></span> | <span data-ttu-id="6920e-133">Идентификатор этой записи об ошибке.</span><span class="sxs-lookup"><span data-stu-id="6920e-133">The identifier of this error entry.</span></span>       |

## <a name="json-representation"></a><span data-ttu-id="6920e-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6920e-134">JSON representation</span></span>
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
