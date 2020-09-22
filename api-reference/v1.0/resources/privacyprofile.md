---
title: Тип ресурса privacyProfile
description: Представляет профиль конфиденциальности организации, который включает URL-адрес заявления о конфиденциальности и сведения о контактном лице, к которому можно обращаться по вопросам, касающимся этого заявления.
localization_priority: Normal
author: davidmu1
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 52aa1171e8fdc1fb01eae0241306fe197d7b36c7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48037222"
---
# <a name="privacyprofile-resource-type"></a><span data-ttu-id="5b941-103">Тип ресурса privacyProfile</span><span class="sxs-lookup"><span data-stu-id="5b941-103">privacyProfile resource type</span></span>

<span data-ttu-id="5b941-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5b941-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5b941-105">Представляет профиль конфиденциальности организации, который включает URL-адрес заявления о конфиденциальности и сведения о контактном лице, к которому можно обращаться по вопросам, касающимся этого заявления.</span><span class="sxs-lookup"><span data-stu-id="5b941-105">Represents a company's privacy profile, which includes a privacy statement URL and a contact person for questions regarding the privacy statement.</span></span>

## <a name="properties"></a><span data-ttu-id="5b941-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="5b941-106">Properties</span></span>
| <span data-ttu-id="5b941-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="5b941-107">Property</span></span>   | <span data-ttu-id="5b941-108">Тип</span><span class="sxs-lookup"><span data-stu-id="5b941-108">Type</span></span>|<span data-ttu-id="5b941-109">Описание</span><span class="sxs-lookup"><span data-stu-id="5b941-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5b941-110">contactEmail</span><span class="sxs-lookup"><span data-stu-id="5b941-110">contactEmail</span></span>|<span data-ttu-id="5b941-111">String</span><span class="sxs-lookup"><span data-stu-id="5b941-111">String</span></span>| <span data-ttu-id="5b941-112">Допустимый электронный адрес SMTP для контактного лица, к которому можно обращаться по вопросам, касающимся заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="5b941-112">A valid smtp email address for the privacy statement contact.</span></span> <span data-ttu-id="5b941-113">Не обязательное.</span><span class="sxs-lookup"><span data-stu-id="5b941-113">Not required.</span></span>|
|<span data-ttu-id="5b941-114">statementUrl</span><span class="sxs-lookup"><span data-stu-id="5b941-114">statementUrl</span></span>|<span data-ttu-id="5b941-115">String</span><span class="sxs-lookup"><span data-stu-id="5b941-115">String</span></span>| <span data-ttu-id="5b941-116">Допустимый формат URL-адреса, который начинается с http:// или https://.</span><span class="sxs-lookup"><span data-stu-id="5b941-116">A valid URL format that begins with http:// or https://.</span></span> <span data-ttu-id="5b941-117">Максимальная длина составляет 255 символов.</span><span class="sxs-lookup"><span data-stu-id="5b941-117">Maximum length is 255 characters.</span></span> <span data-ttu-id="5b941-118">URL-адрес заявления о конфиденциальности организации.</span><span class="sxs-lookup"><span data-stu-id="5b941-118">The URL that directs to the company's privacy statement.</span></span> <span data-ttu-id="5b941-119">Не обязательное.</span><span class="sxs-lookup"><span data-stu-id="5b941-119">Not required.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5b941-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5b941-120">JSON representation</span></span>

<span data-ttu-id="5b941-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5b941-121">Here is a JSON representation of the resource</span></span>

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

