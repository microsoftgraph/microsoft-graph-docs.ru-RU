---
title: Тип ресурса educationSynchronizationError
description: Представляет ошибку во время проверки и/или синхронизации профиля данных учебного заведения. Для каждой записи, которая не проходит проверку и/или синхронизируется с помощью Azure Active Directory (Azure AD), создается уникальная ошибка.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 59650bc56554b9bd4dd7135ae44d53e153c159f8
ms.sourcegitcommit: 2856a818ef3be0d4cfcbc9253906603bcc3d6325
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2020
ms.locfileid: "45434839"
---
# <a name="educationsynchronizationerror-resource-type"></a><span data-ttu-id="411aa-103">Тип ресурса educationSynchronizationError</span><span class="sxs-lookup"><span data-stu-id="411aa-103">educationSynchronizationError resource type</span></span>

<span data-ttu-id="411aa-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="411aa-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="411aa-105">Представляет ошибку во время проверки и/или синхронизации профиля данных учебного заведения. Для каждой записи, которая не проходит проверку и/или синхронизируется с помощью Azure Active Directory (Azure AD), создается уникальная ошибка.</span><span class="sxs-lookup"><span data-stu-id="411aa-105">Represents an error during school data profile validation and/or sync. A unique error is generated for every entry that fails to validate and/or synchronize with Azure Active Directory (Azure AD).</span></span>

## <a name="methods"></a><span data-ttu-id="411aa-106">Методы</span><span class="sxs-lookup"><span data-stu-id="411aa-106">Methods</span></span>

| <span data-ttu-id="411aa-107">Метод</span><span class="sxs-lookup"><span data-stu-id="411aa-107">Method</span></span>                                                                     | <span data-ttu-id="411aa-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="411aa-108">Return Type</span></span>                                  | <span data-ttu-id="411aa-109">Описание</span><span class="sxs-lookup"><span data-stu-id="411aa-109">Description</span></span>                                                           |
| :------------------------------------------------------------------------- | :------------------------------------------- | :-------------------------------------------------------------------- |
| [<span data-ttu-id="411aa-110">Получение ошибок синхронизации</span><span class="sxs-lookup"><span data-stu-id="411aa-110">Get synchronization errors</span></span>](../api/educationsynchronizationerrors-get.md) | <span data-ttu-id="411aa-111">Коллекция **educationSynchronizationError**</span><span class="sxs-lookup"><span data-stu-id="411aa-111">**educationSynchronizationError** collection</span></span> | <span data-ttu-id="411aa-112">Возвращает список ошибок синхронизации, связанных с профилем.</span><span class="sxs-lookup"><span data-stu-id="411aa-112">Returns the list of synchronization errors associated with a profile.</span></span> |

## <a name="properties"></a><span data-ttu-id="411aa-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="411aa-113">Properties</span></span>

| <span data-ttu-id="411aa-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="411aa-114">Property</span></span>             | <span data-ttu-id="411aa-115">Тип</span><span class="sxs-lookup"><span data-stu-id="411aa-115">Type</span></span>           | <span data-ttu-id="411aa-116">Описание</span><span class="sxs-lookup"><span data-stu-id="411aa-116">Description</span></span>                                                     |
| :------------------- | :------------- | :-------------------------------------------------------------- |
| <span data-ttu-id="411aa-117">id</span><span class="sxs-lookup"><span data-stu-id="411aa-117">id</span></span>                   | <span data-ttu-id="411aa-118">Строка</span><span class="sxs-lookup"><span data-stu-id="411aa-118">String</span></span>         | <span data-ttu-id="411aa-119">Уникальный идентификатор ресурса.</span><span class="sxs-lookup"><span data-stu-id="411aa-119">The unique identifier for the resource.</span></span> <span data-ttu-id="411aa-120">(только для чтения)</span><span class="sxs-lookup"><span data-stu-id="411aa-120">(read-only)</span></span>             |
| <span data-ttu-id="411aa-121">ентритипе</span><span class="sxs-lookup"><span data-stu-id="411aa-121">entryType</span></span>            | <span data-ttu-id="411aa-122">Строка</span><span class="sxs-lookup"><span data-stu-id="411aa-122">String</span></span>         | <span data-ttu-id="411aa-123">Представляет объект синхронизации (School, section, Student, преподаватель).</span><span class="sxs-lookup"><span data-stu-id="411aa-123">Represents the sync entity (school, section, student, teacher).</span></span> |
| <span data-ttu-id="411aa-124">errorCode</span><span class="sxs-lookup"><span data-stu-id="411aa-124">errorCode</span></span>            | <span data-ttu-id="411aa-125">String</span><span class="sxs-lookup"><span data-stu-id="411aa-125">String</span></span>         | <span data-ttu-id="411aa-126">Представляет код ошибки для этой ошибки.</span><span class="sxs-lookup"><span data-stu-id="411aa-126">Represents the error code for this error.</span></span>                       |
| <span data-ttu-id="411aa-127">Ошибк</span><span class="sxs-lookup"><span data-stu-id="411aa-127">errorMessage</span></span>         | <span data-ttu-id="411aa-128">Строка</span><span class="sxs-lookup"><span data-stu-id="411aa-128">String</span></span>         | <span data-ttu-id="411aa-129">Содержит описание ошибки.</span><span class="sxs-lookup"><span data-stu-id="411aa-129">Contains a description of the error.</span></span>                            |
| <span data-ttu-id="411aa-130">жоинингвалуе</span><span class="sxs-lookup"><span data-stu-id="411aa-130">joiningValue</span></span>         | <span data-ttu-id="411aa-131">Строка</span><span class="sxs-lookup"><span data-stu-id="411aa-131">String</span></span>         | <span data-ttu-id="411aa-132">Уникальный идентификатор для записи.</span><span class="sxs-lookup"><span data-stu-id="411aa-132">The unique identifier for the entry.</span></span>                            |
| <span data-ttu-id="411aa-133">recordedDateTime</span><span class="sxs-lookup"><span data-stu-id="411aa-133">recordedDateTime</span></span>     | <span data-ttu-id="411aa-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="411aa-134">DateTimeOffset</span></span> | <span data-ttu-id="411aa-135">Время возникновения ошибки.</span><span class="sxs-lookup"><span data-stu-id="411aa-135">The time of occurrence of this error.</span></span>                           |
| <span data-ttu-id="411aa-136">репортаблеидентифиер</span><span class="sxs-lookup"><span data-stu-id="411aa-136">reportableIdentifier</span></span> | <span data-ttu-id="411aa-137">Строка</span><span class="sxs-lookup"><span data-stu-id="411aa-137">String</span></span>         | <span data-ttu-id="411aa-138">Идентификатор этой записи об ошибке.</span><span class="sxs-lookup"><span data-stu-id="411aa-138">The identifier of this error entry.</span></span>                             |

## <a name="json-representation"></a><span data-ttu-id="411aa-139">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="411aa-139">JSON representation</span></span>

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
