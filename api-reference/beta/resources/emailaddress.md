---
title: Тип ресурса emailAddress
description: Представляет имя и SMTP-адрес экземпляра объекта, например сообщения получателю и календарь владельцем.
ms.openlocfilehash: f607fe4ce01b9a3c3f5e7af5aa1638fef3840177
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075846"
---
# <a name="emailaddress-resource-type"></a><span data-ttu-id="2f562-103">Тип ресурса emailAddress</span><span class="sxs-lookup"><span data-stu-id="2f562-103">emailAddress resource type</span></span>

> <span data-ttu-id="2f562-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="2f562-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2f562-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2f562-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2f562-106">Представляет имя и SMTP-адрес экземпляра объекта, например сообщения получателю и календарь владельцем.</span><span class="sxs-lookup"><span data-stu-id="2f562-106">Represents the name and SMTP address of an entity instance, for example, a message recipient or calendar owner.</span></span>

## <a name="properties"></a><span data-ttu-id="2f562-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="2f562-107">Properties</span></span>
| <span data-ttu-id="2f562-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="2f562-108">Property</span></span>     | <span data-ttu-id="2f562-109">Тип</span><span class="sxs-lookup"><span data-stu-id="2f562-109">Type</span></span>   |<span data-ttu-id="2f562-110">Описание</span><span class="sxs-lookup"><span data-stu-id="2f562-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2f562-111">address</span><span class="sxs-lookup"><span data-stu-id="2f562-111">address</span></span>|<span data-ttu-id="2f562-112">String</span><span class="sxs-lookup"><span data-stu-id="2f562-112">String</span></span>|<span data-ttu-id="2f562-113">Адрес электронной почты экземпляр сущности.</span><span class="sxs-lookup"><span data-stu-id="2f562-113">The email address of an entity instance.</span></span>|
|<span data-ttu-id="2f562-114">name</span><span class="sxs-lookup"><span data-stu-id="2f562-114">name</span></span>|<span data-ttu-id="2f562-115">String</span><span class="sxs-lookup"><span data-stu-id="2f562-115">String</span></span>|<span data-ttu-id="2f562-116">Отображаемое имя экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="2f562-116">The display name of an entity instance.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2f562-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2f562-117">JSON representation</span></span>

<span data-ttu-id="2f562-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2f562-118">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.emailAddress"
}-->

```json
{
  "address": "string",
  "name": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "emailAddress resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
