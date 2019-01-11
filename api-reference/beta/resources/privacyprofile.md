---
title: Тип ресурса privacyProfile
description: Представляет профиль конфиденциальности организации, который включает URL-адрес заявления о конфиденциальности и сведения о контактном лице, к которому можно обращаться по вопросам, касающимся этого заявления.
localization_priority: Normal
ms.openlocfilehash: adbd2e04e4d3898de559682b0b87158f938e7252
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27833049"
---
# <a name="privacyprofile-resource-type"></a><span data-ttu-id="64ffc-103">Тип ресурса privacyProfile</span><span class="sxs-lookup"><span data-stu-id="64ffc-103">privacyProfile resource type</span></span>

> <span data-ttu-id="64ffc-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="64ffc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="64ffc-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="64ffc-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="64ffc-106">Представляет профиль конфиденциальности организации, который включает URL-адрес заявления о конфиденциальности и сведения о контактном лице, к которому можно обращаться по вопросам, касающимся этого заявления.</span><span class="sxs-lookup"><span data-stu-id="64ffc-106">Represents a company's privacy profile, which includes a privacy statement URL and a contact person for questions regarding the privacy statement.</span></span>

## <a name="properties"></a><span data-ttu-id="64ffc-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="64ffc-107">Properties</span></span>
| <span data-ttu-id="64ffc-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="64ffc-108">Property</span></span>   | <span data-ttu-id="64ffc-109">Тип</span><span class="sxs-lookup"><span data-stu-id="64ffc-109">Type</span></span>|<span data-ttu-id="64ffc-110">Описание</span><span class="sxs-lookup"><span data-stu-id="64ffc-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="64ffc-111">contactEmail</span><span class="sxs-lookup"><span data-stu-id="64ffc-111">contactEmail</span></span>|<span data-ttu-id="64ffc-112">String</span><span class="sxs-lookup"><span data-stu-id="64ffc-112">String</span></span>| <span data-ttu-id="64ffc-113">Допустимый электронный адрес SMTP для контактного лица, к которому можно обращаться по вопросам, касающимся заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="64ffc-113">A valid smtp email address for the privacy statement contact.</span></span> <span data-ttu-id="64ffc-114">Не обязательное.</span><span class="sxs-lookup"><span data-stu-id="64ffc-114">Not required.</span></span>|
|<span data-ttu-id="64ffc-115">statementUrl</span><span class="sxs-lookup"><span data-stu-id="64ffc-115">statementUrl</span></span>|<span data-ttu-id="64ffc-116">String</span><span class="sxs-lookup"><span data-stu-id="64ffc-116">String</span></span>| <span data-ttu-id="64ffc-117">Допустимый формат URL-адреса, который начинается с http:// или https://.</span><span class="sxs-lookup"><span data-stu-id="64ffc-117">A valid URL format that begins with http:// or https://.</span></span> <span data-ttu-id="64ffc-118">Максимальная длина составляет 255 символов.</span><span class="sxs-lookup"><span data-stu-id="64ffc-118">Maximum length is 255 characters.</span></span> <span data-ttu-id="64ffc-119">URL-адрес заявления о конфиденциальности организации.</span><span class="sxs-lookup"><span data-stu-id="64ffc-119">The URL that directs to the company's privacy statement.</span></span> <span data-ttu-id="64ffc-120">Не обязательное.</span><span class="sxs-lookup"><span data-stu-id="64ffc-120">Not required.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="64ffc-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="64ffc-121">JSON representation</span></span>

<span data-ttu-id="64ffc-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="64ffc-122">Here is a JSON representation of the resource</span></span>

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
