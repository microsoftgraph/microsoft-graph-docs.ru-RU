---
title: Тип ресурса educationSynchronizationError
description: Представляет ошибку во время проверки и/или синхронизации профиля данных учебного заведения. Для каждой записи, которая не проходит проверку и/или синхронизируется с помощью Azure Active Directory (Azure AD), создается уникальная ошибка.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 3c512f921e77468bb30e5109eec29afa9b395b7e
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340536"
---
# <a name="educationsynchronizationerror-resource-type"></a><span data-ttu-id="f9834-103">Тип ресурса educationSynchronizationError</span><span class="sxs-lookup"><span data-stu-id="f9834-103">educationSynchronizationError resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f9834-104">Представляет ошибку во время проверки и/или синхронизации профиля данных учебного заведения. Для каждой записи, которая не проходит проверку и/или синхронизируется с помощью Azure Active Directory (Azure AD), создается уникальная ошибка.</span><span class="sxs-lookup"><span data-stu-id="f9834-104">Represents an error during school data profile validation and/or sync. A unique error is generated for every entry that fails to validate and/or synchronize with Azure Active Directory (Azure AD).</span></span>

## <a name="methods"></a><span data-ttu-id="f9834-105">Методы</span><span class="sxs-lookup"><span data-stu-id="f9834-105">Methods</span></span>

| <span data-ttu-id="f9834-106">Метод</span><span class="sxs-lookup"><span data-stu-id="f9834-106">Method</span></span> | <span data-ttu-id="f9834-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="f9834-107">Return Type</span></span> | <span data-ttu-id="f9834-108">Описание</span><span class="sxs-lookup"><span data-stu-id="f9834-108">Description</span></span> |
|:-|:-|:-|
| [<span data-ttu-id="f9834-109">Получение ошибок синхронизации</span><span class="sxs-lookup"><span data-stu-id="f9834-109">Get synchronization errors</span></span>](../api/educationsynchronizationerrors-get.md) | <span data-ttu-id="f9834-110">Коллекция **educationSynchronizationError**</span><span class="sxs-lookup"><span data-stu-id="f9834-110">**educationSynchronizationError** collection</span></span>| <span data-ttu-id="f9834-111">Возвращает список ошибок синхронизации, связанных с профилем.</span><span class="sxs-lookup"><span data-stu-id="f9834-111">Returns the list of synchronization errors associated with a profile.</span></span> |

## <a name="properties"></a><span data-ttu-id="f9834-112">Свойства</span><span class="sxs-lookup"><span data-stu-id="f9834-112">Properties</span></span>

| <span data-ttu-id="f9834-113">Свойство</span><span class="sxs-lookup"><span data-stu-id="f9834-113">Property</span></span> | <span data-ttu-id="f9834-114">Тип</span><span class="sxs-lookup"><span data-stu-id="f9834-114">Type</span></span> | <span data-ttu-id="f9834-115">Описание</span><span class="sxs-lookup"><span data-stu-id="f9834-115">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="f9834-116">**Ентритипе**</span><span class="sxs-lookup"><span data-stu-id="f9834-116">**entryType**</span></span> | <span data-ttu-id="f9834-117">string</span><span class="sxs-lookup"><span data-stu-id="f9834-117">string</span></span> |  <span data-ttu-id="f9834-118">Представляет объект синхронизации (School, section, Student, преподаватель).</span><span class="sxs-lookup"><span data-stu-id="f9834-118">Represents the sync entity (school, section, student, teacher).</span></span>       |
| <span data-ttu-id="f9834-119">**Коде**</span><span class="sxs-lookup"><span data-stu-id="f9834-119">**errorCode**</span></span> | <span data-ttu-id="f9834-120">string</span><span class="sxs-lookup"><span data-stu-id="f9834-120">string</span></span> |  <span data-ttu-id="f9834-121">Представляет код ошибки для этой ошибки.</span><span class="sxs-lookup"><span data-stu-id="f9834-121">Represents the error code for this error.</span></span>         |
| <span data-ttu-id="f9834-122">**Ошибк**</span><span class="sxs-lookup"><span data-stu-id="f9834-122">**errorMessage**</span></span> | <span data-ttu-id="f9834-123">string</span><span class="sxs-lookup"><span data-stu-id="f9834-123">string</span></span> |  <span data-ttu-id="f9834-124">Содержит описание ошибки.</span><span class="sxs-lookup"><span data-stu-id="f9834-124">Contains a description of the error.</span></span>        |
| <span data-ttu-id="f9834-125">**Жоинингвалуе**</span><span class="sxs-lookup"><span data-stu-id="f9834-125">**joiningValue**</span></span> | <span data-ttu-id="f9834-126">string</span><span class="sxs-lookup"><span data-stu-id="f9834-126">string</span></span> |  <span data-ttu-id="f9834-127">Уникальный идентификатор для записи.</span><span class="sxs-lookup"><span data-stu-id="f9834-127">The unique identifier for the entry.</span></span>         |
| <span data-ttu-id="f9834-128">**recordedDateTime**</span><span class="sxs-lookup"><span data-stu-id="f9834-128">**recordedDateTime**</span></span> | <span data-ttu-id="f9834-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f9834-129">DateTimeOffset</span></span> | <span data-ttu-id="f9834-130">Время возникновения ошибки.</span><span class="sxs-lookup"><span data-stu-id="f9834-130">The time of occurrence of this error.</span></span>         |
| <span data-ttu-id="f9834-131">**Репортаблеидентифиер**</span><span class="sxs-lookup"><span data-stu-id="f9834-131">**reportableIdentifier**</span></span> | <span data-ttu-id="f9834-132">string</span><span class="sxs-lookup"><span data-stu-id="f9834-132">string</span></span> | <span data-ttu-id="f9834-133">Идентификатор этой записи об ошибке.</span><span class="sxs-lookup"><span data-stu-id="f9834-133">The identifier of this error entry.</span></span>       |

## <a name="json-representation"></a><span data-ttu-id="f9834-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f9834-134">JSON representation</span></span>
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
