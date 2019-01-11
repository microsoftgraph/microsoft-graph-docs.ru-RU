---
title: Тип ресурса educationFileSynchronizationVerificationMessage
description: Представляет ошибки, возвращенной клиенту в ответ на запрос на запуск синхронизации профилей на основе CSV школа данных. Этот ресурс будет содержать ошибки, которые возникают из проверки. Пользователям необходимо исправить источника данных, перед перезапуском запроса для синхронизации с Azure Active Directory (Azure AD).
author: mmast-msft
localization_priority: Normal
ms.openlocfilehash: ae09ec3f208adfee64a6392db9732841fc7a0808
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845516"
---
# <a name="educationfilesynchronizationverificationmessage-resource-type"></a><span data-ttu-id="fa8bc-105">Тип ресурса educationFileSynchronizationVerificationMessage</span><span class="sxs-lookup"><span data-stu-id="fa8bc-105">educationFileSynchronizationVerificationMessage resource type</span></span>

> <span data-ttu-id="fa8bc-106">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="fa8bc-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fa8bc-107">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fa8bc-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fa8bc-108">Представляет ошибки, возвращенной клиенту в ответ на запрос на [Запуск синхронизации](../api/educationsynchronizationprofile-start.md) профилей на основе CSV школа данных.</span><span class="sxs-lookup"><span data-stu-id="fa8bc-108">Represents an error returned to the client in response to a request to [start synchronization](../api/educationsynchronizationprofile-start.md) for CSV-based school data profiles.</span></span> <span data-ttu-id="fa8bc-109">Этот ресурс будет содержать ошибки, которые возникают из проверки.</span><span class="sxs-lookup"><span data-stu-id="fa8bc-109">The resource will contain errors that result from the verification.</span></span> <span data-ttu-id="fa8bc-110">Пользователям необходимо исправить источника данных, перед перезапуском запроса для синхронизации с Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="fa8bc-110">Users must fix the source data before you restart the request to synchronize with Azure Active Directory (Azure AD).</span></span>

## <a name="properties"></a><span data-ttu-id="fa8bc-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="fa8bc-111">Properties</span></span>

| <span data-ttu-id="fa8bc-112">Свойство</span><span class="sxs-lookup"><span data-stu-id="fa8bc-112">Property</span></span> | <span data-ttu-id="fa8bc-113">Тип</span><span class="sxs-lookup"><span data-stu-id="fa8bc-113">Type</span></span> | <span data-ttu-id="fa8bc-114">Описание</span><span class="sxs-lookup"><span data-stu-id="fa8bc-114">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="fa8bc-115">**type**</span><span class="sxs-lookup"><span data-stu-id="fa8bc-115">**type**</span></span> | <span data-ttu-id="fa8bc-116">string</span><span class="sxs-lookup"><span data-stu-id="fa8bc-116">string</span></span> | <span data-ttu-id="fa8bc-117">Тип сообщения.</span><span class="sxs-lookup"><span data-stu-id="fa8bc-117">Type of the message.</span></span> <span data-ttu-id="fa8bc-118">Возможные значения: `error`, `warning`, `information`.</span><span class="sxs-lookup"><span data-stu-id="fa8bc-118">Possible values are: `error`, `warning`, `information`.</span></span> | 
| <span data-ttu-id="fa8bc-119">**Имя файла**</span><span class="sxs-lookup"><span data-stu-id="fa8bc-119">**filename**</span></span> | <span data-ttu-id="fa8bc-120">string</span><span class="sxs-lookup"><span data-stu-id="fa8bc-120">string</span></span> | <span data-ttu-id="fa8bc-121">Исходный файл, который содержит ошибки.</span><span class="sxs-lookup"><span data-stu-id="fa8bc-121">Source file that contains the error.</span></span> |
| <span data-ttu-id="fa8bc-122">**description**</span><span class="sxs-lookup"><span data-stu-id="fa8bc-122">**description**</span></span> | <span data-ttu-id="fa8bc-123">строка</span><span class="sxs-lookup"><span data-stu-id="fa8bc-123">string</span></span> | <span data-ttu-id="fa8bc-124">Подробные сведения о типе сообщения.</span><span class="sxs-lookup"><span data-stu-id="fa8bc-124">Detailed information about the message type.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="fa8bc-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fa8bc-125">JSON representation</span></span>

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
