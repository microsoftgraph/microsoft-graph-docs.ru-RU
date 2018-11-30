---
title: Тип ресурса educationSynchronizationError
description: Представляет ошибку во время проверки данных профиля school и/или синхронизации. Уникальный ошибка создается для каждой записи, не удается проверить и/или синхронизация с Azure Active Directory (Azure AD).
ms.openlocfilehash: 91a633ab4056e8e86854a0e2d45ae13e22da19a8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075435"
---
# <a name="educationsynchronizationerror-resource-type"></a><span data-ttu-id="a10f4-103">Тип ресурса educationSynchronizationError</span><span class="sxs-lookup"><span data-stu-id="a10f4-103">educationSynchronizationError resource type</span></span>

> <span data-ttu-id="a10f4-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a10f4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a10f4-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a10f4-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a10f4-106">Представляет ошибку во время проверки данных профиля school и/или синхронизации. Уникальный ошибка создается для каждой записи, не удается проверить и/или синхронизация с Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="a10f4-106">Represents an error during school data profile validation and/or sync. A unique error is generated for every entry that fails to validate and/or synchronize with Azure Active Directory (Azure AD).</span></span>

## <a name="methods"></a><span data-ttu-id="a10f4-107">Методы</span><span class="sxs-lookup"><span data-stu-id="a10f4-107">Methods</span></span>

| <span data-ttu-id="a10f4-108">Метод</span><span class="sxs-lookup"><span data-stu-id="a10f4-108">Method</span></span> | <span data-ttu-id="a10f4-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="a10f4-109">Return Type</span></span> | <span data-ttu-id="a10f4-110">Описание</span><span class="sxs-lookup"><span data-stu-id="a10f4-110">Description</span></span> |
|:-|:-|:-|
| [<span data-ttu-id="a10f4-111">Получение ошибки синхронизации</span><span class="sxs-lookup"><span data-stu-id="a10f4-111">Get synchronization errors</span></span>](../api/educationsynchronizationerrors-get.md) | <span data-ttu-id="a10f4-112">**educationSynchronizationError** коллекции</span><span class="sxs-lookup"><span data-stu-id="a10f4-112">**educationSynchronizationError** collection</span></span>| <span data-ttu-id="a10f4-113">Возвращает список ошибок синхронизации службы, связанные с профилем.</span><span class="sxs-lookup"><span data-stu-id="a10f4-113">Returns the list of synchronization errors associated with a profile.</span></span> |

## <a name="properties"></a><span data-ttu-id="a10f4-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="a10f4-114">Properties</span></span>

| <span data-ttu-id="a10f4-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="a10f4-115">Property</span></span> | <span data-ttu-id="a10f4-116">Тип</span><span class="sxs-lookup"><span data-stu-id="a10f4-116">Type</span></span> | <span data-ttu-id="a10f4-117">Description</span><span class="sxs-lookup"><span data-stu-id="a10f4-117">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="a10f4-118">**entryType**</span><span class="sxs-lookup"><span data-stu-id="a10f4-118">**entryType**</span></span> | <span data-ttu-id="a10f4-119">string</span><span class="sxs-lookup"><span data-stu-id="a10f4-119">string</span></span> |  <span data-ttu-id="a10f4-120">Представляет сущности синхронизации (школа, раздел, учебы, преподаватель).</span><span class="sxs-lookup"><span data-stu-id="a10f4-120">Represents the sync entity (school, section, student, teacher).</span></span>       |
| <span data-ttu-id="a10f4-121">**errorCode**</span><span class="sxs-lookup"><span data-stu-id="a10f4-121">**errorCode**</span></span> | <span data-ttu-id="a10f4-122">string</span><span class="sxs-lookup"><span data-stu-id="a10f4-122">string</span></span> |  <span data-ttu-id="a10f4-123">Представляет код ошибки для этой ошибки.</span><span class="sxs-lookup"><span data-stu-id="a10f4-123">Represents the error code for this error.</span></span>         |
| <span data-ttu-id="a10f4-124">**сообщение об ошибке**</span><span class="sxs-lookup"><span data-stu-id="a10f4-124">**errorMessage**</span></span> | <span data-ttu-id="a10f4-125">string</span><span class="sxs-lookup"><span data-stu-id="a10f4-125">string</span></span> |  <span data-ttu-id="a10f4-126">Содержит описание ошибки.</span><span class="sxs-lookup"><span data-stu-id="a10f4-126">Contains a description of the error.</span></span>        |
| <span data-ttu-id="a10f4-127">**joiningValue**</span><span class="sxs-lookup"><span data-stu-id="a10f4-127">**joiningValue**</span></span> | <span data-ttu-id="a10f4-128">string</span><span class="sxs-lookup"><span data-stu-id="a10f4-128">string</span></span> |  <span data-ttu-id="a10f4-129">Уникальный идентификатор для записи.</span><span class="sxs-lookup"><span data-stu-id="a10f4-129">The unique identifier for the entry.</span></span>         |
| <span data-ttu-id="a10f4-130">**recordedDateTime**</span><span class="sxs-lookup"><span data-stu-id="a10f4-130">**recordedDateTime**</span></span> | <span data-ttu-id="a10f4-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a10f4-131">DateTimeOffset</span></span> | <span data-ttu-id="a10f4-132">Время возникновения этой ошибки.</span><span class="sxs-lookup"><span data-stu-id="a10f4-132">The time of occurrence of this error.</span></span>         |
| <span data-ttu-id="a10f4-133">**reportableIdentifier**</span><span class="sxs-lookup"><span data-stu-id="a10f4-133">**reportableIdentifier**</span></span> | <span data-ttu-id="a10f4-134">string</span><span class="sxs-lookup"><span data-stu-id="a10f4-134">string</span></span> | <span data-ttu-id="a10f4-135">Идентификатор элемента в этой записи об ошибках.</span><span class="sxs-lookup"><span data-stu-id="a10f4-135">The identifier of this error entry.</span></span>       |

## <a name="json-representation"></a><span data-ttu-id="a10f4-136">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a10f4-136">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "#microsoft.graph.educationSynchronizationError"
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
