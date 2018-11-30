---
title: Тип ресурса privacyProfile
description: Представляет профиль конфиденциальности организации, который включает URL-адрес заявления о конфиденциальности и сведения о контактном лице, к которому можно обращаться по вопросам, касающимся этого заявления.
ms.openlocfilehash: fb9d5f929f1c9ae28687b80e987dc0909387f5d6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27082434"
---
# <a name="privacyprofile-resource-type"></a><span data-ttu-id="9747f-103">Тип ресурса privacyProfile</span><span class="sxs-lookup"><span data-stu-id="9747f-103">privacyProfile resource type</span></span>

> <span data-ttu-id="9747f-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="9747f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9747f-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9747f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9747f-106">Представляет профиль конфиденциальности организации, который включает URL-адрес заявления о конфиденциальности и сведения о контактном лице, к которому можно обращаться по вопросам, касающимся этого заявления.</span><span class="sxs-lookup"><span data-stu-id="9747f-106">Represents a company's privacy profile, which includes a privacy statement URL and a contact person for questions regarding the privacy statement.</span></span>

## <a name="properties"></a><span data-ttu-id="9747f-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="9747f-107">Properties</span></span>
| <span data-ttu-id="9747f-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="9747f-108">Property</span></span>   | <span data-ttu-id="9747f-109">Тип</span><span class="sxs-lookup"><span data-stu-id="9747f-109">Type</span></span>|<span data-ttu-id="9747f-110">Описание</span><span class="sxs-lookup"><span data-stu-id="9747f-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9747f-111">contactEmail</span><span class="sxs-lookup"><span data-stu-id="9747f-111">contactEmail</span></span>|<span data-ttu-id="9747f-112">String</span><span class="sxs-lookup"><span data-stu-id="9747f-112">String</span></span>| <span data-ttu-id="9747f-113">Допустимый электронный адрес SMTP для контактного лица, к которому можно обращаться по вопросам, касающимся заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="9747f-113">A valid smtp email address for the privacy statement contact.</span></span> <span data-ttu-id="9747f-114">Не обязательное.</span><span class="sxs-lookup"><span data-stu-id="9747f-114">Not required.</span></span>|
|<span data-ttu-id="9747f-115">statementUrl</span><span class="sxs-lookup"><span data-stu-id="9747f-115">statementUrl</span></span>|<span data-ttu-id="9747f-116">String</span><span class="sxs-lookup"><span data-stu-id="9747f-116">String</span></span>| <span data-ttu-id="9747f-117">Допустимый формат URL-адреса, который начинается с http:// или https://.</span><span class="sxs-lookup"><span data-stu-id="9747f-117">A valid URL format that begins with http:// or https://.</span></span> <span data-ttu-id="9747f-118">Максимальная длина составляет 255 символов.</span><span class="sxs-lookup"><span data-stu-id="9747f-118">Maximum length is 255 characters.</span></span> <span data-ttu-id="9747f-119">URL-адрес заявления о конфиденциальности организации.</span><span class="sxs-lookup"><span data-stu-id="9747f-119">The URL that directs to the company's privacy statement.</span></span> <span data-ttu-id="9747f-120">Не обязательное.</span><span class="sxs-lookup"><span data-stu-id="9747f-120">Not required.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9747f-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9747f-121">JSON representation</span></span>

<span data-ttu-id="9747f-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9747f-122">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.privacyProfile"
}-->

```json
{
  "contactEmail": "string",
  "statementUrl": "string"
}
```