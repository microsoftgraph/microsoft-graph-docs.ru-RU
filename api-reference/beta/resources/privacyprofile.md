---
title: Тип ресурса privacyProfile
description: Представляет профиль конфиденциальности организации, который включает URL-адрес заявления о конфиденциальности и сведения о контактном лице, к которому можно обращаться по вопросам, касающимся этого заявления.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: e43064fe520f100d582e740302a7606c9824b3f2
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521567"
---
# <a name="privacyprofile-resource-type"></a><span data-ttu-id="d10e4-103">Тип ресурса privacyProfile</span><span class="sxs-lookup"><span data-stu-id="d10e4-103">privacyProfile resource type</span></span>

<span data-ttu-id="d10e4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d10e4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d10e4-105">Представляет профиль конфиденциальности организации, который включает URL-адрес заявления о конфиденциальности и сведения о контактном лице, к которому можно обращаться по вопросам, касающимся этого заявления.</span><span class="sxs-lookup"><span data-stu-id="d10e4-105">Represents a company's privacy profile, which includes a privacy statement URL and a contact person for questions regarding the privacy statement.</span></span>

## <a name="properties"></a><span data-ttu-id="d10e4-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="d10e4-106">Properties</span></span>
| <span data-ttu-id="d10e4-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="d10e4-107">Property</span></span>   | <span data-ttu-id="d10e4-108">Тип</span><span class="sxs-lookup"><span data-stu-id="d10e4-108">Type</span></span>|<span data-ttu-id="d10e4-109">Описание</span><span class="sxs-lookup"><span data-stu-id="d10e4-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d10e4-110">contactEmail</span><span class="sxs-lookup"><span data-stu-id="d10e4-110">contactEmail</span></span>|<span data-ttu-id="d10e4-111">String</span><span class="sxs-lookup"><span data-stu-id="d10e4-111">String</span></span>| <span data-ttu-id="d10e4-112">Допустимый электронный адрес SMTP для контактного лица, к которому можно обращаться по вопросам, касающимся заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="d10e4-112">A valid smtp email address for the privacy statement contact.</span></span> <span data-ttu-id="d10e4-113">Не требуется.</span><span class="sxs-lookup"><span data-stu-id="d10e4-113">Not required.</span></span>|
|<span data-ttu-id="d10e4-114">statementUrl</span><span class="sxs-lookup"><span data-stu-id="d10e4-114">statementUrl</span></span>|<span data-ttu-id="d10e4-115">String</span><span class="sxs-lookup"><span data-stu-id="d10e4-115">String</span></span>| <span data-ttu-id="d10e4-116">Допустимый формат URL-адреса, который начинается с http:// или https://.</span><span class="sxs-lookup"><span data-stu-id="d10e4-116">A valid URL format that begins with http:// or https://.</span></span> <span data-ttu-id="d10e4-117">Максимальная длина составляет 255 символов.</span><span class="sxs-lookup"><span data-stu-id="d10e4-117">Maximum length is 255 characters.</span></span> <span data-ttu-id="d10e4-118">URL-адрес заявления о конфиденциальности организации.</span><span class="sxs-lookup"><span data-stu-id="d10e4-118">The URL that directs to the company's privacy statement.</span></span> <span data-ttu-id="d10e4-119">Не обязательное.</span><span class="sxs-lookup"><span data-stu-id="d10e4-119">Not required.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d10e4-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d10e4-120">JSON representation</span></span>

<span data-ttu-id="d10e4-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d10e4-121">Here is a JSON representation of the resource</span></span>

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
