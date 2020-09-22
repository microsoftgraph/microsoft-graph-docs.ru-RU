---
title: Тип ресурса Едукатионфилесинчронизатионверификатионмессаже
description: Представляет ошибку, возвращаемую клиенту в ответ на запрос о запуске синхронизации профилей учебных данных на основе CSV. В ресурсе будут содержаться ошибки, возникающие в результате проверки. Пользователи должны исправить исходные данные перед перезапуском запроса на синхронизацию с Azure Active Directory (Azure AD).
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: b65335538453f35457d5e83c49f7ba7c830d6a43
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48095450"
---
# <a name="educationfilesynchronizationverificationmessage-resource-type"></a><span data-ttu-id="68e00-105">Тип ресурса Едукатионфилесинчронизатионверификатионмессаже</span><span class="sxs-lookup"><span data-stu-id="68e00-105">educationFileSynchronizationVerificationMessage resource type</span></span>

<span data-ttu-id="68e00-106">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="68e00-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="68e00-107">Представляет ошибку, возвращаемую клиенту в ответ на запрос о [запуске синхронизации](../api/educationsynchronizationprofile-start.md) профилей учебных данных на основе CSV.</span><span class="sxs-lookup"><span data-stu-id="68e00-107">Represents an error returned to the client in response to a request to [start synchronization](../api/educationsynchronizationprofile-start.md) for CSV-based school data profiles.</span></span> <span data-ttu-id="68e00-108">В ресурсе будут содержаться ошибки, возникающие в результате проверки.</span><span class="sxs-lookup"><span data-stu-id="68e00-108">The resource will contain errors that result from the verification.</span></span> <span data-ttu-id="68e00-109">Пользователи должны исправить исходные данные перед перезапуском запроса на синхронизацию с Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="68e00-109">Users must fix the source data before you restart the request to synchronize with Azure Active Directory (Azure AD).</span></span>

## <a name="properties"></a><span data-ttu-id="68e00-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="68e00-110">Properties</span></span>

| <span data-ttu-id="68e00-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="68e00-111">Property</span></span>    | <span data-ttu-id="68e00-112">Тип</span><span class="sxs-lookup"><span data-stu-id="68e00-112">Type</span></span>   | <span data-ttu-id="68e00-113">Описание</span><span class="sxs-lookup"><span data-stu-id="68e00-113">Description</span></span>                                                                  |
| :---------- | :----- | :--------------------------------------------------------------------------- |
| <span data-ttu-id="68e00-114">type</span><span class="sxs-lookup"><span data-stu-id="68e00-114">type</span></span>        | <span data-ttu-id="68e00-115">string</span><span class="sxs-lookup"><span data-stu-id="68e00-115">string</span></span> | <span data-ttu-id="68e00-116">Тип сообщения.</span><span class="sxs-lookup"><span data-stu-id="68e00-116">Type of the message.</span></span> <span data-ttu-id="68e00-117">Возможные значения: `error`, `warning`, `information`.</span><span class="sxs-lookup"><span data-stu-id="68e00-117">Possible values are: `error`, `warning`, `information`.</span></span> |
| <span data-ttu-id="68e00-118">задан</span><span class="sxs-lookup"><span data-stu-id="68e00-118">filename</span></span>    | <span data-ttu-id="68e00-119">string</span><span class="sxs-lookup"><span data-stu-id="68e00-119">string</span></span> | <span data-ttu-id="68e00-120">Исходный файл, который содержит ошибку.</span><span class="sxs-lookup"><span data-stu-id="68e00-120">Source file that contains the error.</span></span>                                         |
| <span data-ttu-id="68e00-121">description</span><span class="sxs-lookup"><span data-stu-id="68e00-121">description</span></span> | <span data-ttu-id="68e00-122">string</span><span class="sxs-lookup"><span data-stu-id="68e00-122">string</span></span> | <span data-ttu-id="68e00-123">Подробные сведения о типе сообщения.</span><span class="sxs-lookup"><span data-stu-id="68e00-123">Detailed information about the message type.</span></span>                                 |

## <a name="json-representation"></a><span data-ttu-id="68e00-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="68e00-124">JSON representation</span></span>

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


