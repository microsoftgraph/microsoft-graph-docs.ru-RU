---
title: Тип ресурса educationSynchronizationError
description: Представляет ошибку во время проверки и/или синхронизации профиля данных учебного заведения. Для каждой записи, которая не проходит проверку и/или синхронизируется с помощью Azure Active Directory (Azure AD), создается уникальная ошибка.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: d46d1160ae59174d9fcb4df89559531e3a032e55
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42500326"
---
# <a name="educationsynchronizationerror-resource-type"></a><span data-ttu-id="0b3e6-103">Тип ресурса educationSynchronizationError</span><span class="sxs-lookup"><span data-stu-id="0b3e6-103">educationSynchronizationError resource type</span></span>

<span data-ttu-id="0b3e6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0b3e6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0b3e6-105">Представляет ошибку во время проверки и/или синхронизации профиля данных учебного заведения. Для каждой записи, которая не проходит проверку и/или синхронизируется с помощью Azure Active Directory (Azure AD), создается уникальная ошибка.</span><span class="sxs-lookup"><span data-stu-id="0b3e6-105">Represents an error during school data profile validation and/or sync. A unique error is generated for every entry that fails to validate and/or synchronize with Azure Active Directory (Azure AD).</span></span>

## <a name="methods"></a><span data-ttu-id="0b3e6-106">Методы</span><span class="sxs-lookup"><span data-stu-id="0b3e6-106">Methods</span></span>

| <span data-ttu-id="0b3e6-107">Метод</span><span class="sxs-lookup"><span data-stu-id="0b3e6-107">Method</span></span> | <span data-ttu-id="0b3e6-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="0b3e6-108">Return Type</span></span> | <span data-ttu-id="0b3e6-109">Описание</span><span class="sxs-lookup"><span data-stu-id="0b3e6-109">Description</span></span> |
|:-|:-|:-|
| [<span data-ttu-id="0b3e6-110">Получение ошибок синхронизации</span><span class="sxs-lookup"><span data-stu-id="0b3e6-110">Get synchronization errors</span></span>](../api/educationsynchronizationerrors-get.md) | <span data-ttu-id="0b3e6-111">Коллекция **educationSynchronizationError**</span><span class="sxs-lookup"><span data-stu-id="0b3e6-111">**educationSynchronizationError** collection</span></span>| <span data-ttu-id="0b3e6-112">Возвращает список ошибок синхронизации, связанных с профилем.</span><span class="sxs-lookup"><span data-stu-id="0b3e6-112">Returns the list of synchronization errors associated with a profile.</span></span> |

## <a name="properties"></a><span data-ttu-id="0b3e6-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="0b3e6-113">Properties</span></span>

| <span data-ttu-id="0b3e6-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="0b3e6-114">Property</span></span> | <span data-ttu-id="0b3e6-115">Тип</span><span class="sxs-lookup"><span data-stu-id="0b3e6-115">Type</span></span> | <span data-ttu-id="0b3e6-116">Описание</span><span class="sxs-lookup"><span data-stu-id="0b3e6-116">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="0b3e6-117">**ентритипе**</span><span class="sxs-lookup"><span data-stu-id="0b3e6-117">**entryType**</span></span> | <span data-ttu-id="0b3e6-118">string</span><span class="sxs-lookup"><span data-stu-id="0b3e6-118">string</span></span> |  <span data-ttu-id="0b3e6-119">Представляет объект синхронизации (School, section, Student, преподаватель).</span><span class="sxs-lookup"><span data-stu-id="0b3e6-119">Represents the sync entity (school, section, student, teacher).</span></span>       |
| <span data-ttu-id="0b3e6-120">**errorCode**</span><span class="sxs-lookup"><span data-stu-id="0b3e6-120">**errorCode**</span></span> | <span data-ttu-id="0b3e6-121">string</span><span class="sxs-lookup"><span data-stu-id="0b3e6-121">string</span></span> |  <span data-ttu-id="0b3e6-122">Представляет код ошибки для этой ошибки.</span><span class="sxs-lookup"><span data-stu-id="0b3e6-122">Represents the error code for this error.</span></span>         |
| <span data-ttu-id="0b3e6-123">**Ошибк**</span><span class="sxs-lookup"><span data-stu-id="0b3e6-123">**errorMessage**</span></span> | <span data-ttu-id="0b3e6-124">string</span><span class="sxs-lookup"><span data-stu-id="0b3e6-124">string</span></span> |  <span data-ttu-id="0b3e6-125">Содержит описание ошибки.</span><span class="sxs-lookup"><span data-stu-id="0b3e6-125">Contains a description of the error.</span></span>        |
| <span data-ttu-id="0b3e6-126">**жоинингвалуе**</span><span class="sxs-lookup"><span data-stu-id="0b3e6-126">**joiningValue**</span></span> | <span data-ttu-id="0b3e6-127">string</span><span class="sxs-lookup"><span data-stu-id="0b3e6-127">string</span></span> |  <span data-ttu-id="0b3e6-128">Уникальный идентификатор для записи.</span><span class="sxs-lookup"><span data-stu-id="0b3e6-128">The unique identifier for the entry.</span></span>         |
| <span data-ttu-id="0b3e6-129">**recordedDateTime**</span><span class="sxs-lookup"><span data-stu-id="0b3e6-129">**recordedDateTime**</span></span> | <span data-ttu-id="0b3e6-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0b3e6-130">DateTimeOffset</span></span> | <span data-ttu-id="0b3e6-131">Время возникновения ошибки.</span><span class="sxs-lookup"><span data-stu-id="0b3e6-131">The time of occurrence of this error.</span></span>         |
| <span data-ttu-id="0b3e6-132">**репортаблеидентифиер**</span><span class="sxs-lookup"><span data-stu-id="0b3e6-132">**reportableIdentifier**</span></span> | <span data-ttu-id="0b3e6-133">string</span><span class="sxs-lookup"><span data-stu-id="0b3e6-133">string</span></span> | <span data-ttu-id="0b3e6-134">Идентификатор этой записи об ошибке.</span><span class="sxs-lookup"><span data-stu-id="0b3e6-134">The identifier of this error entry.</span></span>       |

## <a name="json-representation"></a><span data-ttu-id="0b3e6-135">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0b3e6-135">JSON representation</span></span>
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
