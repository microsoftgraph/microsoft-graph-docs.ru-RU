---
title: Тип ресурса privacyProfile
description: Представляет профиль конфиденциальности организации, который включает URL-адрес заявления о конфиденциальности и сведения о контактном лице, к которому можно обращаться по вопросам, касающимся этого заявления.
localization_priority: Normal
ms.openlocfilehash: 29c4a01cde0e05c42ce74576e769ca005840e854
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27884982"
---
# <a name="privacyprofile-resource-type"></a><span data-ttu-id="69433-103">Тип ресурса privacyProfile</span><span class="sxs-lookup"><span data-stu-id="69433-103">privacyProfile resource type</span></span>

<span data-ttu-id="69433-104">Представляет профиль конфиденциальности организации, который включает URL-адрес заявления о конфиденциальности и сведения о контактном лице, к которому можно обращаться по вопросам, касающимся этого заявления.</span><span class="sxs-lookup"><span data-stu-id="69433-104">Represents a company's privacy profile, which includes a privacy statement URL and a contact person for questions regarding the privacy statement.</span></span>

## <a name="properties"></a><span data-ttu-id="69433-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="69433-105">Properties</span></span>
| <span data-ttu-id="69433-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="69433-106">Property</span></span>   | <span data-ttu-id="69433-107">Тип</span><span class="sxs-lookup"><span data-stu-id="69433-107">Type</span></span>|<span data-ttu-id="69433-108">Описание</span><span class="sxs-lookup"><span data-stu-id="69433-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="69433-109">contactEmail</span><span class="sxs-lookup"><span data-stu-id="69433-109">contactEmail</span></span>|<span data-ttu-id="69433-110">String</span><span class="sxs-lookup"><span data-stu-id="69433-110">String</span></span>| <span data-ttu-id="69433-111">Допустимый электронный адрес SMTP для контактного лица, к которому можно обращаться по вопросам, касающимся заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="69433-111">A valid smtp email address for the privacy statement contact.</span></span> <span data-ttu-id="69433-112">Не обязательное.</span><span class="sxs-lookup"><span data-stu-id="69433-112">Not required.</span></span>|
|<span data-ttu-id="69433-113">statementUrl</span><span class="sxs-lookup"><span data-stu-id="69433-113">statementUrl</span></span>|<span data-ttu-id="69433-114">String</span><span class="sxs-lookup"><span data-stu-id="69433-114">String</span></span>| <span data-ttu-id="69433-115">Допустимый формат URL-адреса, который начинается с http:// или https://.</span><span class="sxs-lookup"><span data-stu-id="69433-115">A valid URL format that begins with http:// or https://.</span></span> <span data-ttu-id="69433-116">Максимальная длина составляет 255 символов.</span><span class="sxs-lookup"><span data-stu-id="69433-116">Maximum length is 255 characters.</span></span> <span data-ttu-id="69433-117">URL-адрес заявления о конфиденциальности организации.</span><span class="sxs-lookup"><span data-stu-id="69433-117">The URL that directs to the company's privacy statement.</span></span> <span data-ttu-id="69433-118">Не обязательное.</span><span class="sxs-lookup"><span data-stu-id="69433-118">Not required.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="69433-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="69433-119">JSON representation</span></span>

<span data-ttu-id="69433-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="69433-120">Here is a JSON representation of the resource</span></span>

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
