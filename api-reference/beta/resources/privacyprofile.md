---
title: Тип ресурса privacyProfile
description: Представляет профиль конфиденциальности организации, который включает URL-адрес заявления о конфиденциальности и сведения о контактном лице, к которому можно обращаться по вопросам, касающимся этого заявления.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: davidmu1
ms.openlocfilehash: 14ec9ae7119743e1b206f2d4b748cec09b9bfd3e
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46811464"
---
# <a name="privacyprofile-resource-type"></a><span data-ttu-id="4c9c3-103">Тип ресурса privacyProfile</span><span class="sxs-lookup"><span data-stu-id="4c9c3-103">privacyProfile resource type</span></span>

<span data-ttu-id="4c9c3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4c9c3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4c9c3-105">Представляет профиль конфиденциальности организации, который включает URL-адрес заявления о конфиденциальности и сведения о контактном лице, к которому можно обращаться по вопросам, касающимся этого заявления.</span><span class="sxs-lookup"><span data-stu-id="4c9c3-105">Represents a company's privacy profile, which includes a privacy statement URL and a contact person for questions regarding the privacy statement.</span></span>

## <a name="properties"></a><span data-ttu-id="4c9c3-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="4c9c3-106">Properties</span></span>
| <span data-ttu-id="4c9c3-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="4c9c3-107">Property</span></span>   | <span data-ttu-id="4c9c3-108">Тип</span><span class="sxs-lookup"><span data-stu-id="4c9c3-108">Type</span></span>|<span data-ttu-id="4c9c3-109">Описание</span><span class="sxs-lookup"><span data-stu-id="4c9c3-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4c9c3-110">contactEmail</span><span class="sxs-lookup"><span data-stu-id="4c9c3-110">contactEmail</span></span>|<span data-ttu-id="4c9c3-111">String</span><span class="sxs-lookup"><span data-stu-id="4c9c3-111">String</span></span>| <span data-ttu-id="4c9c3-112">Допустимый электронный адрес SMTP для контактного лица, к которому можно обращаться по вопросам, касающимся заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="4c9c3-112">A valid smtp email address for the privacy statement contact.</span></span> <span data-ttu-id="4c9c3-113">Не обязательное.</span><span class="sxs-lookup"><span data-stu-id="4c9c3-113">Not required.</span></span>|
|<span data-ttu-id="4c9c3-114">statementUrl</span><span class="sxs-lookup"><span data-stu-id="4c9c3-114">statementUrl</span></span>|<span data-ttu-id="4c9c3-115">String</span><span class="sxs-lookup"><span data-stu-id="4c9c3-115">String</span></span>| <span data-ttu-id="4c9c3-116">Допустимый формат URL-адреса, который начинается с http:// или https://.</span><span class="sxs-lookup"><span data-stu-id="4c9c3-116">A valid URL format that begins with http:// or https://.</span></span> <span data-ttu-id="4c9c3-117">Максимальная длина составляет 255 символов.</span><span class="sxs-lookup"><span data-stu-id="4c9c3-117">Maximum length is 255 characters.</span></span> <span data-ttu-id="4c9c3-118">URL-адрес заявления о конфиденциальности организации.</span><span class="sxs-lookup"><span data-stu-id="4c9c3-118">The URL that directs to the company's privacy statement.</span></span> <span data-ttu-id="4c9c3-119">Не обязательное.</span><span class="sxs-lookup"><span data-stu-id="4c9c3-119">Not required.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4c9c3-120">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="4c9c3-120">JSON representation</span></span>

<span data-ttu-id="4c9c3-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4c9c3-121">Here is a JSON representation of the resource</span></span>

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
