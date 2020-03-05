---
title: Тип ресурса Едукатионфилесинчронизатионверификатионмессаже
description: Представляет ошибку, возвращаемую клиенту в ответ на запрос о запуске синхронизации профилей учебных данных на основе CSV. В ресурсе будут содержаться ошибки, возникающие в результате проверки. Пользователи должны исправить исходные данные перед перезапуском запроса на синхронизацию с Azure Active Directory (Azure AD).
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 45f439adaf45ade7e63dd4cde8ed72852244192c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42502013"
---
# <a name="educationfilesynchronizationverificationmessage-resource-type"></a><span data-ttu-id="b0a3b-105">Тип ресурса Едукатионфилесинчронизатионверификатионмессаже</span><span class="sxs-lookup"><span data-stu-id="b0a3b-105">educationFileSynchronizationVerificationMessage resource type</span></span>

<span data-ttu-id="b0a3b-106">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="b0a3b-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b0a3b-107">Представляет ошибку, возвращаемую клиенту в ответ на запрос о [запуске синхронизации](../api/educationsynchronizationprofile-start.md) профилей учебных данных на основе CSV.</span><span class="sxs-lookup"><span data-stu-id="b0a3b-107">Represents an error returned to the client in response to a request to [start synchronization](../api/educationsynchronizationprofile-start.md) for CSV-based school data profiles.</span></span> <span data-ttu-id="b0a3b-108">В ресурсе будут содержаться ошибки, возникающие в результате проверки.</span><span class="sxs-lookup"><span data-stu-id="b0a3b-108">The resource will contain errors that result from the verification.</span></span> <span data-ttu-id="b0a3b-109">Пользователи должны исправить исходные данные перед перезапуском запроса на синхронизацию с Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="b0a3b-109">Users must fix the source data before you restart the request to synchronize with Azure Active Directory (Azure AD).</span></span>

## <a name="properties"></a><span data-ttu-id="b0a3b-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="b0a3b-110">Properties</span></span>

| <span data-ttu-id="b0a3b-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="b0a3b-111">Property</span></span> | <span data-ttu-id="b0a3b-112">Тип</span><span class="sxs-lookup"><span data-stu-id="b0a3b-112">Type</span></span> | <span data-ttu-id="b0a3b-113">Описание</span><span class="sxs-lookup"><span data-stu-id="b0a3b-113">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="b0a3b-114">**type**</span><span class="sxs-lookup"><span data-stu-id="b0a3b-114">**type**</span></span> | <span data-ttu-id="b0a3b-115">string</span><span class="sxs-lookup"><span data-stu-id="b0a3b-115">string</span></span> | <span data-ttu-id="b0a3b-116">Тип сообщения.</span><span class="sxs-lookup"><span data-stu-id="b0a3b-116">Type of the message.</span></span> <span data-ttu-id="b0a3b-117">Возможные значения: `error`, `warning`, `information`.</span><span class="sxs-lookup"><span data-stu-id="b0a3b-117">Possible values are: `error`, `warning`, `information`.</span></span> | 
| <span data-ttu-id="b0a3b-118">**задан**</span><span class="sxs-lookup"><span data-stu-id="b0a3b-118">**filename**</span></span> | <span data-ttu-id="b0a3b-119">строка</span><span class="sxs-lookup"><span data-stu-id="b0a3b-119">string</span></span> | <span data-ttu-id="b0a3b-120">Исходный файл, который содержит ошибку.</span><span class="sxs-lookup"><span data-stu-id="b0a3b-120">Source file that contains the error.</span></span> |
| <span data-ttu-id="b0a3b-121">**description**</span><span class="sxs-lookup"><span data-stu-id="b0a3b-121">**description**</span></span> | <span data-ttu-id="b0a3b-122">строка</span><span class="sxs-lookup"><span data-stu-id="b0a3b-122">string</span></span> | <span data-ttu-id="b0a3b-123">Подробные сведения о типе сообщения.</span><span class="sxs-lookup"><span data-stu-id="b0a3b-123">Detailed information about the message type.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b0a3b-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b0a3b-124">JSON representation</span></span>

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
