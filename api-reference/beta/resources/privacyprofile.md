---
title: Тип ресурса privacyProfile
description: Представляет профиль конфиденциальности организации, который включает URL-адрес заявления о конфиденциальности и сведения о контактном лице, к которому можно обращаться по вопросам, касающимся этого заявления.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 29036620ad571566b5e3535891a9bb5ed92ad9cf
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008938"
---
# <a name="privacyprofile-resource-type"></a><span data-ttu-id="b2134-103">Тип ресурса privacyProfile</span><span class="sxs-lookup"><span data-stu-id="b2134-103">privacyProfile resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b2134-104">Представляет профиль конфиденциальности организации, который включает URL-адрес заявления о конфиденциальности и сведения о контактном лице, к которому можно обращаться по вопросам, касающимся этого заявления.</span><span class="sxs-lookup"><span data-stu-id="b2134-104">Represents a company's privacy profile, which includes a privacy statement URL and a contact person for questions regarding the privacy statement.</span></span>

## <a name="properties"></a><span data-ttu-id="b2134-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="b2134-105">Properties</span></span>
| <span data-ttu-id="b2134-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="b2134-106">Property</span></span>   | <span data-ttu-id="b2134-107">Тип</span><span class="sxs-lookup"><span data-stu-id="b2134-107">Type</span></span>|<span data-ttu-id="b2134-108">Описание</span><span class="sxs-lookup"><span data-stu-id="b2134-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b2134-109">contactEmail</span><span class="sxs-lookup"><span data-stu-id="b2134-109">contactEmail</span></span>|<span data-ttu-id="b2134-110">String</span><span class="sxs-lookup"><span data-stu-id="b2134-110">String</span></span>| <span data-ttu-id="b2134-111">Допустимый электронный адрес SMTP для контактного лица, к которому можно обращаться по вопросам, касающимся заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="b2134-111">A valid smtp email address for the privacy statement contact.</span></span> <span data-ttu-id="b2134-112">Не требуется.</span><span class="sxs-lookup"><span data-stu-id="b2134-112">Not required.</span></span>|
|<span data-ttu-id="b2134-113">statementUrl</span><span class="sxs-lookup"><span data-stu-id="b2134-113">statementUrl</span></span>|<span data-ttu-id="b2134-114">String</span><span class="sxs-lookup"><span data-stu-id="b2134-114">String</span></span>| <span data-ttu-id="b2134-115">Допустимый формат URL-адреса, который начинается с http:// или https://.</span><span class="sxs-lookup"><span data-stu-id="b2134-115">A valid URL format that begins with http:// or https://.</span></span> <span data-ttu-id="b2134-116">Максимальная длина составляет 255 символов.</span><span class="sxs-lookup"><span data-stu-id="b2134-116">Maximum length is 255 characters.</span></span> <span data-ttu-id="b2134-117">URL-адрес заявления о конфиденциальности организации.</span><span class="sxs-lookup"><span data-stu-id="b2134-117">The URL that directs to the company's privacy statement.</span></span> <span data-ttu-id="b2134-118">Не обязательное.</span><span class="sxs-lookup"><span data-stu-id="b2134-118">Not required.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b2134-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b2134-119">JSON representation</span></span>

<span data-ttu-id="b2134-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b2134-120">Here is a JSON representation of the resource</span></span>

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
