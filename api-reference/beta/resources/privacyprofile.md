---
title: Тип ресурса privacyProfile
description: Представляет профиль конфиденциальности организации, который включает URL-адрес заявления о конфиденциальности и сведения о контактном лице, к которому можно обращаться по вопросам, касающимся этого заявления.
localization_priority: Normal
ms.openlocfilehash: 9c110cbdb8a456b43936d3b56db5d4563686ed6e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510122"
---
# <a name="privacyprofile-resource-type"></a><span data-ttu-id="71576-103">Тип ресурса privacyProfile</span><span class="sxs-lookup"><span data-stu-id="71576-103">privacyProfile resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="71576-104">Представляет профиль конфиденциальности организации, который включает URL-адрес заявления о конфиденциальности и сведения о контактном лице, к которому можно обращаться по вопросам, касающимся этого заявления.</span><span class="sxs-lookup"><span data-stu-id="71576-104">Represents a company's privacy profile, which includes a privacy statement URL and a contact person for questions regarding the privacy statement.</span></span>

## <a name="properties"></a><span data-ttu-id="71576-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="71576-105">Properties</span></span>
| <span data-ttu-id="71576-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="71576-106">Property</span></span>   | <span data-ttu-id="71576-107">Тип</span><span class="sxs-lookup"><span data-stu-id="71576-107">Type</span></span>|<span data-ttu-id="71576-108">Описание</span><span class="sxs-lookup"><span data-stu-id="71576-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="71576-109">contactEmail</span><span class="sxs-lookup"><span data-stu-id="71576-109">contactEmail</span></span>|<span data-ttu-id="71576-110">String</span><span class="sxs-lookup"><span data-stu-id="71576-110">String</span></span>| <span data-ttu-id="71576-111">Допустимый электронный адрес SMTP для контактного лица, к которому можно обращаться по вопросам, касающимся заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="71576-111">A valid smtp email address for the privacy statement contact.</span></span> <span data-ttu-id="71576-112">Не обязательное.</span><span class="sxs-lookup"><span data-stu-id="71576-112">Not required.</span></span>|
|<span data-ttu-id="71576-113">statementUrl</span><span class="sxs-lookup"><span data-stu-id="71576-113">statementUrl</span></span>|<span data-ttu-id="71576-114">String</span><span class="sxs-lookup"><span data-stu-id="71576-114">String</span></span>| <span data-ttu-id="71576-115">Допустимый формат URL-адреса, который начинается с http:// или https://.</span><span class="sxs-lookup"><span data-stu-id="71576-115">A valid URL format that begins with http:// or https://.</span></span> <span data-ttu-id="71576-116">Максимальная длина составляет 255 символов.</span><span class="sxs-lookup"><span data-stu-id="71576-116">Maximum length is 255 characters.</span></span> <span data-ttu-id="71576-117">URL-адрес заявления о конфиденциальности организации.</span><span class="sxs-lookup"><span data-stu-id="71576-117">The URL that directs to the company's privacy statement.</span></span> <span data-ttu-id="71576-118">Не обязательное.</span><span class="sxs-lookup"><span data-stu-id="71576-118">Not required.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="71576-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="71576-119">JSON representation</span></span>

<span data-ttu-id="71576-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="71576-120">Here is a JSON representation of the resource</span></span>

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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/privacyprofile.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
