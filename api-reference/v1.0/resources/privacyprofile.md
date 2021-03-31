---
title: Тип ресурса privacyProfile
description: Представляет профиль конфиденциальности организации, который включает URL-адрес заявления о конфиденциальности и сведения о контактном лице, к которому можно обращаться по вопросам, касающимся этого заявления.
localization_priority: Normal
author: Jumaodhiss
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: a64defb220a6c8adc28ba06cd205c1eb70496329
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469432"
---
# <a name="privacyprofile-resource-type"></a><span data-ttu-id="55e30-103">Тип ресурса privacyProfile</span><span class="sxs-lookup"><span data-stu-id="55e30-103">privacyProfile resource type</span></span>

<span data-ttu-id="55e30-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="55e30-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="55e30-105">Представляет профиль конфиденциальности организации, который включает URL-адрес заявления о конфиденциальности и сведения о контактном лице, к которому можно обращаться по вопросам, касающимся этого заявления.</span><span class="sxs-lookup"><span data-stu-id="55e30-105">Represents a company's privacy profile, which includes a privacy statement URL and a contact person for questions regarding the privacy statement.</span></span>

## <a name="properties"></a><span data-ttu-id="55e30-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="55e30-106">Properties</span></span>
| <span data-ttu-id="55e30-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="55e30-107">Property</span></span>   | <span data-ttu-id="55e30-108">Тип</span><span class="sxs-lookup"><span data-stu-id="55e30-108">Type</span></span>|<span data-ttu-id="55e30-109">Описание</span><span class="sxs-lookup"><span data-stu-id="55e30-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="55e30-110">contactEmail</span><span class="sxs-lookup"><span data-stu-id="55e30-110">contactEmail</span></span>|<span data-ttu-id="55e30-111">String</span><span class="sxs-lookup"><span data-stu-id="55e30-111">String</span></span>| <span data-ttu-id="55e30-112">Допустимый электронный адрес SMTP для контактного лица, к которому можно обращаться по вопросам, касающимся заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="55e30-112">A valid smtp email address for the privacy statement contact.</span></span> <span data-ttu-id="55e30-113">Не обязательное.</span><span class="sxs-lookup"><span data-stu-id="55e30-113">Not required.</span></span>|
|<span data-ttu-id="55e30-114">statementUrl</span><span class="sxs-lookup"><span data-stu-id="55e30-114">statementUrl</span></span>|<span data-ttu-id="55e30-115">String</span><span class="sxs-lookup"><span data-stu-id="55e30-115">String</span></span>| <span data-ttu-id="55e30-116">Допустимый формат URL-адреса, который начинается с http:// или https://.</span><span class="sxs-lookup"><span data-stu-id="55e30-116">A valid URL format that begins with http:// or https://.</span></span> <span data-ttu-id="55e30-117">Максимальная длина составляет 255 символов.</span><span class="sxs-lookup"><span data-stu-id="55e30-117">Maximum length is 255 characters.</span></span> <span data-ttu-id="55e30-118">URL-адрес заявления о конфиденциальности организации.</span><span class="sxs-lookup"><span data-stu-id="55e30-118">The URL that directs to the company's privacy statement.</span></span> <span data-ttu-id="55e30-119">Не обязательное.</span><span class="sxs-lookup"><span data-stu-id="55e30-119">Not required.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="55e30-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="55e30-120">JSON representation</span></span>

<span data-ttu-id="55e30-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="55e30-121">Here is a JSON representation of the resource</span></span>

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

