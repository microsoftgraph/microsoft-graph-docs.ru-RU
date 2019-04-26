---
title: Тип ресурса Едукатионфилесинчронизатионверификатионмессаже
description: Представляет ошибку, возвращаемую клиенту в ответ на запрос о запуске синхронизации профилей учебных данных на основе CSV. В ресурсе будут содержаться ошибки, возникающие в результате проверки. Пользователи должны исправить исходные данные перед перезапуском запроса на синхронизацию с Azure Active Directory (Azure AD).
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: bbf38f15fbe14112ef254c625a8747e57eb1cae4
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340526"
---
# <a name="educationfilesynchronizationverificationmessage-resource-type"></a><span data-ttu-id="cbd73-105">Тип ресурса Едукатионфилесинчронизатионверификатионмессаже</span><span class="sxs-lookup"><span data-stu-id="cbd73-105">educationFileSynchronizationVerificationMessage resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cbd73-106">Представляет ошибку, возвращаемую клиенту в ответ на запрос о [запуске синхронизации](../api/educationsynchronizationprofile-start.md) профилей учебных данных на основе CSV.</span><span class="sxs-lookup"><span data-stu-id="cbd73-106">Represents an error returned to the client in response to a request to [start synchronization](../api/educationsynchronizationprofile-start.md) for CSV-based school data profiles.</span></span> <span data-ttu-id="cbd73-107">В ресурсе будут содержаться ошибки, возникающие в результате проверки.</span><span class="sxs-lookup"><span data-stu-id="cbd73-107">The resource will contain errors that result from the verification.</span></span> <span data-ttu-id="cbd73-108">Пользователи должны исправить исходные данные перед перезапуском запроса на синхронизацию с Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="cbd73-108">Users must fix the source data before you restart the request to synchronize with Azure Active Directory (Azure AD).</span></span>

## <a name="properties"></a><span data-ttu-id="cbd73-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="cbd73-109">Properties</span></span>

| <span data-ttu-id="cbd73-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="cbd73-110">Property</span></span> | <span data-ttu-id="cbd73-111">Тип</span><span class="sxs-lookup"><span data-stu-id="cbd73-111">Type</span></span> | <span data-ttu-id="cbd73-112">Описание</span><span class="sxs-lookup"><span data-stu-id="cbd73-112">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="cbd73-113">**type**</span><span class="sxs-lookup"><span data-stu-id="cbd73-113">**type**</span></span> | <span data-ttu-id="cbd73-114">string</span><span class="sxs-lookup"><span data-stu-id="cbd73-114">string</span></span> | <span data-ttu-id="cbd73-115">Тип сообщения.</span><span class="sxs-lookup"><span data-stu-id="cbd73-115">Type of the message.</span></span> <span data-ttu-id="cbd73-116">Возможные значения: `error`, `warning`, `information`.</span><span class="sxs-lookup"><span data-stu-id="cbd73-116">Possible values are: `error`, `warning`, `information`.</span></span> | 
| <span data-ttu-id="cbd73-117">**задан**</span><span class="sxs-lookup"><span data-stu-id="cbd73-117">**filename**</span></span> | <span data-ttu-id="cbd73-118">string</span><span class="sxs-lookup"><span data-stu-id="cbd73-118">string</span></span> | <span data-ttu-id="cbd73-119">Исходный файл, который содержит ошибку.</span><span class="sxs-lookup"><span data-stu-id="cbd73-119">Source file that contains the error.</span></span> |
| <span data-ttu-id="cbd73-120">**description**</span><span class="sxs-lookup"><span data-stu-id="cbd73-120">**description**</span></span> | <span data-ttu-id="cbd73-121">string</span><span class="sxs-lookup"><span data-stu-id="cbd73-121">string</span></span> | <span data-ttu-id="cbd73-122">Подробные сведения о типе сообщения.</span><span class="sxs-lookup"><span data-stu-id="cbd73-122">Detailed information about the message type.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="cbd73-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cbd73-123">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationFileSynchronizationVerificationMessage"
}-->

```json
{
    "type": "String",
    "fileName": "String",
    "description": "String"
}
```
