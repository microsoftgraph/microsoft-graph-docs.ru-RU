---
title: Тип ресурса educationSynchronizationError
description: Представляет ошибку во время проверки и/или синхронизации профиля данных учебного заведения. Для каждой записи, которая не проходит проверку и/или синхронизируется с помощью Azure Active Directory (Azure AD), создается уникальная ошибка.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 2af4ef9f17452714373d42b67af6e87a7f87fe1d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47989650"
---
# <a name="educationsynchronizationerror-resource-type"></a><span data-ttu-id="78c3e-103">Тип ресурса educationSynchronizationError</span><span class="sxs-lookup"><span data-stu-id="78c3e-103">educationSynchronizationError resource type</span></span>

<span data-ttu-id="78c3e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="78c3e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="78c3e-105">Представляет ошибку во время проверки и/или синхронизации профиля данных учебного заведения. Для каждой записи, которая не проходит проверку и/или синхронизируется с помощью Azure Active Directory (Azure AD), создается уникальная ошибка.</span><span class="sxs-lookup"><span data-stu-id="78c3e-105">Represents an error during school data profile validation and/or sync. A unique error is generated for every entry that fails to validate and/or synchronize with Azure Active Directory (Azure AD).</span></span>

## <a name="methods"></a><span data-ttu-id="78c3e-106">Методы</span><span class="sxs-lookup"><span data-stu-id="78c3e-106">Methods</span></span>

| <span data-ttu-id="78c3e-107">Метод</span><span class="sxs-lookup"><span data-stu-id="78c3e-107">Method</span></span>                                                                     | <span data-ttu-id="78c3e-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="78c3e-108">Return Type</span></span>                                  | <span data-ttu-id="78c3e-109">Описание</span><span class="sxs-lookup"><span data-stu-id="78c3e-109">Description</span></span>                                                           |
| :------------------------------------------------------------------------- | :------------------------------------------- | :-------------------------------------------------------------------- |
| [<span data-ttu-id="78c3e-110">Получение ошибок синхронизации</span><span class="sxs-lookup"><span data-stu-id="78c3e-110">Get synchronization errors</span></span>](../api/educationsynchronizationerrors-get.md) | <span data-ttu-id="78c3e-111">Коллекция **educationSynchronizationError**</span><span class="sxs-lookup"><span data-stu-id="78c3e-111">**educationSynchronizationError** collection</span></span> | <span data-ttu-id="78c3e-112">Возвращает список ошибок синхронизации, связанных с профилем.</span><span class="sxs-lookup"><span data-stu-id="78c3e-112">Returns the list of synchronization errors associated with a profile.</span></span> |

## <a name="properties"></a><span data-ttu-id="78c3e-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="78c3e-113">Properties</span></span>

| <span data-ttu-id="78c3e-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="78c3e-114">Property</span></span>             | <span data-ttu-id="78c3e-115">Тип</span><span class="sxs-lookup"><span data-stu-id="78c3e-115">Type</span></span>           | <span data-ttu-id="78c3e-116">Описание</span><span class="sxs-lookup"><span data-stu-id="78c3e-116">Description</span></span>                                                     |
| :------------------- | :------------- | :-------------------------------------------------------------- |
| <span data-ttu-id="78c3e-117">id</span><span class="sxs-lookup"><span data-stu-id="78c3e-117">id</span></span>                   | <span data-ttu-id="78c3e-118">String</span><span class="sxs-lookup"><span data-stu-id="78c3e-118">String</span></span>         | <span data-ttu-id="78c3e-119">Уникальный идентификатор ресурса.</span><span class="sxs-lookup"><span data-stu-id="78c3e-119">The unique identifier for the resource.</span></span> <span data-ttu-id="78c3e-120">(только для чтения)</span><span class="sxs-lookup"><span data-stu-id="78c3e-120">(read-only)</span></span>             |
| <span data-ttu-id="78c3e-121">ентритипе</span><span class="sxs-lookup"><span data-stu-id="78c3e-121">entryType</span></span>            | <span data-ttu-id="78c3e-122">String</span><span class="sxs-lookup"><span data-stu-id="78c3e-122">String</span></span>         | <span data-ttu-id="78c3e-123">Представляет объект синхронизации (School, section, Student, преподаватель).</span><span class="sxs-lookup"><span data-stu-id="78c3e-123">Represents the sync entity (school, section, student, teacher).</span></span> |
| <span data-ttu-id="78c3e-124">errorCode</span><span class="sxs-lookup"><span data-stu-id="78c3e-124">errorCode</span></span>            | <span data-ttu-id="78c3e-125">String</span><span class="sxs-lookup"><span data-stu-id="78c3e-125">String</span></span>         | <span data-ttu-id="78c3e-126">Представляет код ошибки для этой ошибки.</span><span class="sxs-lookup"><span data-stu-id="78c3e-126">Represents the error code for this error.</span></span>                       |
| <span data-ttu-id="78c3e-127">Ошибк</span><span class="sxs-lookup"><span data-stu-id="78c3e-127">errorMessage</span></span>         | <span data-ttu-id="78c3e-128">String</span><span class="sxs-lookup"><span data-stu-id="78c3e-128">String</span></span>         | <span data-ttu-id="78c3e-129">Содержит описание ошибки.</span><span class="sxs-lookup"><span data-stu-id="78c3e-129">Contains a description of the error.</span></span>                            |
| <span data-ttu-id="78c3e-130">жоинингвалуе</span><span class="sxs-lookup"><span data-stu-id="78c3e-130">joiningValue</span></span>         | <span data-ttu-id="78c3e-131">String</span><span class="sxs-lookup"><span data-stu-id="78c3e-131">String</span></span>         | <span data-ttu-id="78c3e-132">Уникальный идентификатор для записи.</span><span class="sxs-lookup"><span data-stu-id="78c3e-132">The unique identifier for the entry.</span></span>                            |
| <span data-ttu-id="78c3e-133">recordedDateTime</span><span class="sxs-lookup"><span data-stu-id="78c3e-133">recordedDateTime</span></span>     | <span data-ttu-id="78c3e-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="78c3e-134">DateTimeOffset</span></span> | <span data-ttu-id="78c3e-135">Время возникновения ошибки.</span><span class="sxs-lookup"><span data-stu-id="78c3e-135">The time of occurrence of this error.</span></span>                           |
| <span data-ttu-id="78c3e-136">репортаблеидентифиер</span><span class="sxs-lookup"><span data-stu-id="78c3e-136">reportableIdentifier</span></span> | <span data-ttu-id="78c3e-137">String</span><span class="sxs-lookup"><span data-stu-id="78c3e-137">String</span></span>         | <span data-ttu-id="78c3e-138">Идентификатор этой записи об ошибке.</span><span class="sxs-lookup"><span data-stu-id="78c3e-138">The identifier of this error entry.</span></span>                             |

## <a name="json-representation"></a><span data-ttu-id="78c3e-139">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="78c3e-139">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSynchronizationError"
}-->

```json
{
  "id": "String",
  "entryType": "String",
  "errorCode": "String",
  "errorMessage": "String",
  "joiningValue": "String",
  "recordedDateTime": "DateTimeOffset",
  "reportableIdentifier": "String"
}
```


