---
title: Тип ресурса privacyProfile
description: Представляет профиль конфиденциальности организации, который включает URL-адрес заявления о конфиденциальности и сведения о контактном лице, к которому можно обращаться по вопросам, касающимся этого заявления.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 02942e654eb198986d765489e2f35b75e2611e92
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035093"
---
# <a name="privacyprofile-resource-type"></a><span data-ttu-id="f4866-103">Тип ресурса privacyProfile</span><span class="sxs-lookup"><span data-stu-id="f4866-103">privacyProfile resource type</span></span>

<span data-ttu-id="f4866-104">Представляет профиль конфиденциальности организации, который включает URL-адрес заявления о конфиденциальности и сведения о контактном лице, к которому можно обращаться по вопросам, касающимся этого заявления.</span><span class="sxs-lookup"><span data-stu-id="f4866-104">Represents a company's privacy profile, which includes a privacy statement URL and a contact person for questions regarding the privacy statement.</span></span>

## <a name="properties"></a><span data-ttu-id="f4866-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="f4866-105">Properties</span></span>
| <span data-ttu-id="f4866-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="f4866-106">Property</span></span>   | <span data-ttu-id="f4866-107">Тип</span><span class="sxs-lookup"><span data-stu-id="f4866-107">Type</span></span>|<span data-ttu-id="f4866-108">Описание</span><span class="sxs-lookup"><span data-stu-id="f4866-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f4866-109">contactEmail</span><span class="sxs-lookup"><span data-stu-id="f4866-109">contactEmail</span></span>|<span data-ttu-id="f4866-110">String</span><span class="sxs-lookup"><span data-stu-id="f4866-110">String</span></span>| <span data-ttu-id="f4866-111">Допустимый электронный адрес SMTP для контактного лица, к которому можно обращаться по вопросам, касающимся заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="f4866-111">A valid smtp email address for the privacy statement contact.</span></span> <span data-ttu-id="f4866-112">Не требуется.</span><span class="sxs-lookup"><span data-stu-id="f4866-112">Not required.</span></span>|
|<span data-ttu-id="f4866-113">statementUrl</span><span class="sxs-lookup"><span data-stu-id="f4866-113">statementUrl</span></span>|<span data-ttu-id="f4866-114">String</span><span class="sxs-lookup"><span data-stu-id="f4866-114">String</span></span>| <span data-ttu-id="f4866-115">Допустимый формат URL-адреса, который начинается с http:// или https://.</span><span class="sxs-lookup"><span data-stu-id="f4866-115">A valid URL format that begins with http:// or https://.</span></span> <span data-ttu-id="f4866-116">Максимальная длина составляет 255 символов.</span><span class="sxs-lookup"><span data-stu-id="f4866-116">Maximum length is 255 characters.</span></span> <span data-ttu-id="f4866-117">URL-адрес заявления о конфиденциальности организации.</span><span class="sxs-lookup"><span data-stu-id="f4866-117">The URL that directs to the company's privacy statement.</span></span> <span data-ttu-id="f4866-118">Не обязательное.</span><span class="sxs-lookup"><span data-stu-id="f4866-118">Not required.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f4866-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f4866-119">JSON representation</span></span>

<span data-ttu-id="f4866-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f4866-120">Here is a JSON representation of the resource</span></span>

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
