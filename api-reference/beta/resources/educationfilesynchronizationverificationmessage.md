---
title: Тип ресурса educationFileSynchronizationVerificationMessage
description: Представляет ошибки, возвращенной клиенту в ответ на запрос на запуск синхронизации профилей на основе CSV школа данных. Этот ресурс будет содержать ошибки, которые возникают из проверки. Пользователям необходимо исправить источника данных, перед перезапуском запроса для синхронизации с Azure Active Directory (Azure AD).
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 26f96c83ce14539011664b446265328f714ed402
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529896"
---
# <a name="educationfilesynchronizationverificationmessage-resource-type"></a><span data-ttu-id="79dfd-105">Тип ресурса educationFileSynchronizationVerificationMessage</span><span class="sxs-lookup"><span data-stu-id="79dfd-105">educationFileSynchronizationVerificationMessage resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="79dfd-106">Представляет ошибки, возвращенной клиенту в ответ на запрос на [Запуск синхронизации](../api/educationsynchronizationprofile-start.md) профилей на основе CSV школа данных.</span><span class="sxs-lookup"><span data-stu-id="79dfd-106">Represents an error returned to the client in response to a request to [start synchronization](../api/educationsynchronizationprofile-start.md) for CSV-based school data profiles.</span></span> <span data-ttu-id="79dfd-107">Этот ресурс будет содержать ошибки, которые возникают из проверки.</span><span class="sxs-lookup"><span data-stu-id="79dfd-107">The resource will contain errors that result from the verification.</span></span> <span data-ttu-id="79dfd-108">Пользователям необходимо исправить источника данных, перед перезапуском запроса для синхронизации с Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="79dfd-108">Users must fix the source data before you restart the request to synchronize with Azure Active Directory (Azure AD).</span></span>

## <a name="properties"></a><span data-ttu-id="79dfd-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="79dfd-109">Properties</span></span>

| <span data-ttu-id="79dfd-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="79dfd-110">Property</span></span> | <span data-ttu-id="79dfd-111">Тип</span><span class="sxs-lookup"><span data-stu-id="79dfd-111">Type</span></span> | <span data-ttu-id="79dfd-112">Описание</span><span class="sxs-lookup"><span data-stu-id="79dfd-112">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="79dfd-113">**type**</span><span class="sxs-lookup"><span data-stu-id="79dfd-113">**type**</span></span> | <span data-ttu-id="79dfd-114">string</span><span class="sxs-lookup"><span data-stu-id="79dfd-114">string</span></span> | <span data-ttu-id="79dfd-115">Тип сообщения.</span><span class="sxs-lookup"><span data-stu-id="79dfd-115">Type of the message.</span></span> <span data-ttu-id="79dfd-116">Возможные значения: `error`, `warning`, `information`.</span><span class="sxs-lookup"><span data-stu-id="79dfd-116">Possible values are: `error`, `warning`, `information`.</span></span> | 
| <span data-ttu-id="79dfd-117">**fileName**</span><span class="sxs-lookup"><span data-stu-id="79dfd-117">**filename**</span></span> | <span data-ttu-id="79dfd-118">string</span><span class="sxs-lookup"><span data-stu-id="79dfd-118">string</span></span> | <span data-ttu-id="79dfd-119">Исходный файл, который содержит ошибки.</span><span class="sxs-lookup"><span data-stu-id="79dfd-119">Source file that contains the error.</span></span> |
| <span data-ttu-id="79dfd-120">**description**</span><span class="sxs-lookup"><span data-stu-id="79dfd-120">**description**</span></span> | <span data-ttu-id="79dfd-121">строка</span><span class="sxs-lookup"><span data-stu-id="79dfd-121">string</span></span> | <span data-ttu-id="79dfd-122">Подробные сведения о типе сообщения.</span><span class="sxs-lookup"><span data-stu-id="79dfd-122">Detailed information about the message type.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="79dfd-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="79dfd-123">JSON representation</span></span>

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
