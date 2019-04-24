---
title: Тип ресурса Едукатионфилесинчронизатионверификатионмессаже
description: Представляет ошибку, возвращаемую клиенту в ответ на запрос о запуске синхронизации профилей учебных данных на основе CSV. В ресурсе будут содержаться ошибки, возникающие в результате проверки. Пользователи должны исправить исходные данные перед перезапуском запроса на синхронизацию с Azure Active Directory (Azure AD).
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 26f96c83ce14539011664b446265328f714ed402
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32507133"
---
# <a name="educationfilesynchronizationverificationmessage-resource-type"></a><span data-ttu-id="2a6bf-105">Тип ресурса Едукатионфилесинчронизатионверификатионмессаже</span><span class="sxs-lookup"><span data-stu-id="2a6bf-105">educationFileSynchronizationVerificationMessage resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2a6bf-106">Представляет ошибку, возвращаемую клиенту в ответ на запрос о [запуске синхронизации](../api/educationsynchronizationprofile-start.md) профилей учебных данных на основе CSV.</span><span class="sxs-lookup"><span data-stu-id="2a6bf-106">Represents an error returned to the client in response to a request to [start synchronization](../api/educationsynchronizationprofile-start.md) for CSV-based school data profiles.</span></span> <span data-ttu-id="2a6bf-107">В ресурсе будут содержаться ошибки, возникающие в результате проверки.</span><span class="sxs-lookup"><span data-stu-id="2a6bf-107">The resource will contain errors that result from the verification.</span></span> <span data-ttu-id="2a6bf-108">Пользователи должны исправить исходные данные перед перезапуском запроса на синхронизацию с Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="2a6bf-108">Users must fix the source data before you restart the request to synchronize with Azure Active Directory (Azure AD).</span></span>

## <a name="properties"></a><span data-ttu-id="2a6bf-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="2a6bf-109">Properties</span></span>

| <span data-ttu-id="2a6bf-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="2a6bf-110">Property</span></span> | <span data-ttu-id="2a6bf-111">Тип</span><span class="sxs-lookup"><span data-stu-id="2a6bf-111">Type</span></span> | <span data-ttu-id="2a6bf-112">Описание</span><span class="sxs-lookup"><span data-stu-id="2a6bf-112">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="2a6bf-113">**type**</span><span class="sxs-lookup"><span data-stu-id="2a6bf-113">**type**</span></span> | <span data-ttu-id="2a6bf-114">string</span><span class="sxs-lookup"><span data-stu-id="2a6bf-114">string</span></span> | <span data-ttu-id="2a6bf-115">Тип сообщения.</span><span class="sxs-lookup"><span data-stu-id="2a6bf-115">Type of the message.</span></span> <span data-ttu-id="2a6bf-116">Возможные значения: `error`, `warning`, `information`.</span><span class="sxs-lookup"><span data-stu-id="2a6bf-116">Possible values are: `error`, `warning`, `information`.</span></span> | 
| <span data-ttu-id="2a6bf-117">**задан**</span><span class="sxs-lookup"><span data-stu-id="2a6bf-117">**filename**</span></span> | <span data-ttu-id="2a6bf-118">строка</span><span class="sxs-lookup"><span data-stu-id="2a6bf-118">string</span></span> | <span data-ttu-id="2a6bf-119">Исходный файл, который содержит ошибку.</span><span class="sxs-lookup"><span data-stu-id="2a6bf-119">Source file that contains the error.</span></span> |
| <span data-ttu-id="2a6bf-120">**description**</span><span class="sxs-lookup"><span data-stu-id="2a6bf-120">**description**</span></span> | <span data-ttu-id="2a6bf-121">строка</span><span class="sxs-lookup"><span data-stu-id="2a6bf-121">string</span></span> | <span data-ttu-id="2a6bf-122">Подробные сведения о типе сообщения.</span><span class="sxs-lookup"><span data-stu-id="2a6bf-122">Detailed information about the message type.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="2a6bf-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2a6bf-123">JSON representation</span></span>

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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationfilesynchronizationverificationmessage.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
