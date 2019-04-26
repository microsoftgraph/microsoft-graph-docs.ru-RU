---
title: Тип ресурса privacyProfile
description: Представляет профиль конфиденциальности организации, который включает URL-адрес заявления о конфиденциальности и сведения о контактном лице, к которому можно обращаться по вопросам, касающимся этого заявления.
localization_priority: Normal
ms.openlocfilehash: d1d7593e5b0f0ef9d4ac36f902ec244e93fd51c1
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344207"
---
# <a name="privacyprofile-resource-type"></a><span data-ttu-id="f0fd5-103">Тип ресурса privacyProfile</span><span class="sxs-lookup"><span data-stu-id="f0fd5-103">privacyProfile resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f0fd5-104">Представляет профиль конфиденциальности организации, который включает URL-адрес заявления о конфиденциальности и сведения о контактном лице, к которому можно обращаться по вопросам, касающимся этого заявления.</span><span class="sxs-lookup"><span data-stu-id="f0fd5-104">Represents a company's privacy profile, which includes a privacy statement URL and a contact person for questions regarding the privacy statement.</span></span>

## <a name="properties"></a><span data-ttu-id="f0fd5-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="f0fd5-105">Properties</span></span>
| <span data-ttu-id="f0fd5-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="f0fd5-106">Property</span></span>   | <span data-ttu-id="f0fd5-107">Тип</span><span class="sxs-lookup"><span data-stu-id="f0fd5-107">Type</span></span>|<span data-ttu-id="f0fd5-108">Описание</span><span class="sxs-lookup"><span data-stu-id="f0fd5-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f0fd5-109">contactEmail</span><span class="sxs-lookup"><span data-stu-id="f0fd5-109">contactEmail</span></span>|<span data-ttu-id="f0fd5-110">String</span><span class="sxs-lookup"><span data-stu-id="f0fd5-110">String</span></span>| <span data-ttu-id="f0fd5-111">Допустимый электронный адрес SMTP для контактного лица, к которому можно обращаться по вопросам, касающимся заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="f0fd5-111">A valid smtp email address for the privacy statement contact.</span></span> <span data-ttu-id="f0fd5-112">Не требуется.</span><span class="sxs-lookup"><span data-stu-id="f0fd5-112">Not required.</span></span>|
|<span data-ttu-id="f0fd5-113">statementUrl</span><span class="sxs-lookup"><span data-stu-id="f0fd5-113">statementUrl</span></span>|<span data-ttu-id="f0fd5-114">String</span><span class="sxs-lookup"><span data-stu-id="f0fd5-114">String</span></span>| <span data-ttu-id="f0fd5-115">Допустимый формат URL-адреса, который начинается с http:// или https://.</span><span class="sxs-lookup"><span data-stu-id="f0fd5-115">A valid URL format that begins with http:// or https://.</span></span> <span data-ttu-id="f0fd5-116">Максимальная длина составляет 255 символов.</span><span class="sxs-lookup"><span data-stu-id="f0fd5-116">Maximum length is 255 characters.</span></span> <span data-ttu-id="f0fd5-117">URL-адрес заявления о конфиденциальности организации.</span><span class="sxs-lookup"><span data-stu-id="f0fd5-117">The URL that directs to the company's privacy statement.</span></span> <span data-ttu-id="f0fd5-118">Не обязательное.</span><span class="sxs-lookup"><span data-stu-id="f0fd5-118">Not required.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f0fd5-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f0fd5-119">JSON representation</span></span>

<span data-ttu-id="f0fd5-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f0fd5-120">Here is a JSON representation of the resource</span></span>

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
