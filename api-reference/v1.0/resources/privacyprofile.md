---
title: Тип ресурса privacyProfile
description: Представляет профиль конфиденциальности организации, который включает URL-адрес заявления о конфиденциальности и сведения о контактном лице, к которому можно обращаться по вопросам, касающимся этого заявления.
ms.openlocfilehash: 5d1a8e48a2d8310f45c71fbc73485e8ec4fe8697
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27027887"
---
# <a name="privacyprofile-resource-type"></a><span data-ttu-id="4f2e0-103">Тип ресурса privacyProfile</span><span class="sxs-lookup"><span data-stu-id="4f2e0-103">privacyProfile resource type</span></span>

<span data-ttu-id="4f2e0-104">Представляет профиль конфиденциальности организации, который включает URL-адрес заявления о конфиденциальности и сведения о контактном лице, к которому можно обращаться по вопросам, касающимся этого заявления.</span><span class="sxs-lookup"><span data-stu-id="4f2e0-104">Represents a company's privacy profile, which includes a privacy statement URL and a contact person for questions regarding the privacy statement.</span></span>

## <a name="properties"></a><span data-ttu-id="4f2e0-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="4f2e0-105">Properties</span></span>
| <span data-ttu-id="4f2e0-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="4f2e0-106">Property</span></span>   | <span data-ttu-id="4f2e0-107">Тип</span><span class="sxs-lookup"><span data-stu-id="4f2e0-107">Type</span></span>|<span data-ttu-id="4f2e0-108">Описание</span><span class="sxs-lookup"><span data-stu-id="4f2e0-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4f2e0-109">contactEmail</span><span class="sxs-lookup"><span data-stu-id="4f2e0-109">contactEmail</span></span>|<span data-ttu-id="4f2e0-110">String</span><span class="sxs-lookup"><span data-stu-id="4f2e0-110">String</span></span>| <span data-ttu-id="4f2e0-111">Допустимый электронный адрес SMTP для контактного лица, к которому можно обращаться по вопросам, касающимся заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="4f2e0-111">A valid smtp email address for the privacy statement contact.</span></span> <span data-ttu-id="4f2e0-112">Не обязательное.</span><span class="sxs-lookup"><span data-stu-id="4f2e0-112">Not required.</span></span>|
|<span data-ttu-id="4f2e0-113">statementUrl</span><span class="sxs-lookup"><span data-stu-id="4f2e0-113">statementUrl</span></span>|<span data-ttu-id="4f2e0-114">String</span><span class="sxs-lookup"><span data-stu-id="4f2e0-114">String</span></span>| <span data-ttu-id="4f2e0-115">Допустимый формат URL-адреса, который начинается с http:// или https://.</span><span class="sxs-lookup"><span data-stu-id="4f2e0-115">A valid URL format that begins with http:// or https://.</span></span> <span data-ttu-id="4f2e0-116">Максимальная длина составляет 255 символов.</span><span class="sxs-lookup"><span data-stu-id="4f2e0-116">Maximum length is 255 characters.</span></span> <span data-ttu-id="4f2e0-117">URL-адрес заявления о конфиденциальности организации.</span><span class="sxs-lookup"><span data-stu-id="4f2e0-117">The URL that directs to the company's privacy statement.</span></span> <span data-ttu-id="4f2e0-118">Не обязательное.</span><span class="sxs-lookup"><span data-stu-id="4f2e0-118">Not required.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4f2e0-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4f2e0-119">JSON representation</span></span>

<span data-ttu-id="4f2e0-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4f2e0-120">Here is a JSON representation of the resource</span></span>

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