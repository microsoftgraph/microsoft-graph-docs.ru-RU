---
title: Тип ресурса privacyProfile
description: Представляет профиль конфиденциальности организации, который включает URL-адрес заявления о конфиденциальности и сведения о контактном лице, к которому можно обращаться по вопросам, касающимся этого заявления.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: directory-management
author: Jumaodhiss
ms.openlocfilehash: df8fce6758fd7e251dd9358a38a8e602b3b4d1ba
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "51467997"
---
# <a name="privacyprofile-resource-type"></a><span data-ttu-id="fbb48-103">Тип ресурса privacyProfile</span><span class="sxs-lookup"><span data-stu-id="fbb48-103">privacyProfile resource type</span></span>

<span data-ttu-id="fbb48-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fbb48-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fbb48-105">Представляет профиль конфиденциальности организации, который включает URL-адрес заявления о конфиденциальности и сведения о контактном лице, к которому можно обращаться по вопросам, касающимся этого заявления.</span><span class="sxs-lookup"><span data-stu-id="fbb48-105">Represents a company's privacy profile, which includes a privacy statement URL and a contact person for questions regarding the privacy statement.</span></span>

## <a name="properties"></a><span data-ttu-id="fbb48-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="fbb48-106">Properties</span></span>
| <span data-ttu-id="fbb48-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="fbb48-107">Property</span></span>   | <span data-ttu-id="fbb48-108">Тип</span><span class="sxs-lookup"><span data-stu-id="fbb48-108">Type</span></span>|<span data-ttu-id="fbb48-109">Описание</span><span class="sxs-lookup"><span data-stu-id="fbb48-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fbb48-110">contactEmail</span><span class="sxs-lookup"><span data-stu-id="fbb48-110">contactEmail</span></span>|<span data-ttu-id="fbb48-111">String</span><span class="sxs-lookup"><span data-stu-id="fbb48-111">String</span></span>| <span data-ttu-id="fbb48-112">Допустимый электронный адрес SMTP для контактного лица, к которому можно обращаться по вопросам, касающимся заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="fbb48-112">A valid smtp email address for the privacy statement contact.</span></span> <span data-ttu-id="fbb48-113">Не обязательное.</span><span class="sxs-lookup"><span data-stu-id="fbb48-113">Not required.</span></span>|
|<span data-ttu-id="fbb48-114">statementUrl</span><span class="sxs-lookup"><span data-stu-id="fbb48-114">statementUrl</span></span>|<span data-ttu-id="fbb48-115">String</span><span class="sxs-lookup"><span data-stu-id="fbb48-115">String</span></span>| <span data-ttu-id="fbb48-116">Допустимый формат URL-адреса, который начинается с http:// или https://.</span><span class="sxs-lookup"><span data-stu-id="fbb48-116">A valid URL format that begins with http:// or https://.</span></span> <span data-ttu-id="fbb48-117">Максимальная длина составляет 255 символов.</span><span class="sxs-lookup"><span data-stu-id="fbb48-117">Maximum length is 255 characters.</span></span> <span data-ttu-id="fbb48-118">URL-адрес заявления о конфиденциальности организации.</span><span class="sxs-lookup"><span data-stu-id="fbb48-118">The URL that directs to the company's privacy statement.</span></span> <span data-ttu-id="fbb48-119">Не обязательное.</span><span class="sxs-lookup"><span data-stu-id="fbb48-119">Not required.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fbb48-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fbb48-120">JSON representation</span></span>

<span data-ttu-id="fbb48-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fbb48-121">Here is a JSON representation of the resource</span></span>

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


