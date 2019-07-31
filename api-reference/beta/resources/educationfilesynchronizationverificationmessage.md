---
title: Тип ресурса Едукатионфилесинчронизатионверификатионмессаже
description: Представляет ошибку, возвращаемую клиенту в ответ на запрос о запуске синхронизации профилей учебных данных на основе CSV. В ресурсе будут содержаться ошибки, возникающие в результате проверки. Пользователи должны исправить исходные данные перед перезапуском запроса на синхронизацию с Azure Active Directory (Azure AD).
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: cf462873226ff4238f95ffc4798b6eb662666f3d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36006411"
---
# <a name="educationfilesynchronizationverificationmessage-resource-type"></a><span data-ttu-id="a154c-105">Тип ресурса Едукатионфилесинчронизатионверификатионмессаже</span><span class="sxs-lookup"><span data-stu-id="a154c-105">educationFileSynchronizationVerificationMessage resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a154c-106">Представляет ошибку, возвращаемую клиенту в ответ на запрос о [запуске синхронизации](../api/educationsynchronizationprofile-start.md) профилей учебных данных на основе CSV.</span><span class="sxs-lookup"><span data-stu-id="a154c-106">Represents an error returned to the client in response to a request to [start synchronization](../api/educationsynchronizationprofile-start.md) for CSV-based school data profiles.</span></span> <span data-ttu-id="a154c-107">В ресурсе будут содержаться ошибки, возникающие в результате проверки.</span><span class="sxs-lookup"><span data-stu-id="a154c-107">The resource will contain errors that result from the verification.</span></span> <span data-ttu-id="a154c-108">Пользователи должны исправить исходные данные перед перезапуском запроса на синхронизацию с Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="a154c-108">Users must fix the source data before you restart the request to synchronize with Azure Active Directory (Azure AD).</span></span>

## <a name="properties"></a><span data-ttu-id="a154c-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="a154c-109">Properties</span></span>

| <span data-ttu-id="a154c-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="a154c-110">Property</span></span> | <span data-ttu-id="a154c-111">Тип</span><span class="sxs-lookup"><span data-stu-id="a154c-111">Type</span></span> | <span data-ttu-id="a154c-112">Описание</span><span class="sxs-lookup"><span data-stu-id="a154c-112">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="a154c-113">**type**</span><span class="sxs-lookup"><span data-stu-id="a154c-113">**type**</span></span> | <span data-ttu-id="a154c-114">string</span><span class="sxs-lookup"><span data-stu-id="a154c-114">string</span></span> | <span data-ttu-id="a154c-115">Тип сообщения.</span><span class="sxs-lookup"><span data-stu-id="a154c-115">Type of the message.</span></span> <span data-ttu-id="a154c-116">Возможные значения: `error`, `warning`, `information`.</span><span class="sxs-lookup"><span data-stu-id="a154c-116">Possible values are: `error`, `warning`, `information`.</span></span> | 
| <span data-ttu-id="a154c-117">**задан**</span><span class="sxs-lookup"><span data-stu-id="a154c-117">**filename**</span></span> | <span data-ttu-id="a154c-118">string</span><span class="sxs-lookup"><span data-stu-id="a154c-118">string</span></span> | <span data-ttu-id="a154c-119">Исходный файл, который содержит ошибку.</span><span class="sxs-lookup"><span data-stu-id="a154c-119">Source file that contains the error.</span></span> |
| <span data-ttu-id="a154c-120">**description**</span><span class="sxs-lookup"><span data-stu-id="a154c-120">**description**</span></span> | <span data-ttu-id="a154c-121">string</span><span class="sxs-lookup"><span data-stu-id="a154c-121">string</span></span> | <span data-ttu-id="a154c-122">Подробные сведения о типе сообщения.</span><span class="sxs-lookup"><span data-stu-id="a154c-122">Detailed information about the message type.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a154c-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a154c-123">JSON representation</span></span>

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
