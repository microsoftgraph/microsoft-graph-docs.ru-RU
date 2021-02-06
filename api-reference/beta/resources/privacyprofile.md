---
title: Тип ресурса privacyProfile
description: Представляет профиль конфиденциальности организации, который включает URL-адрес заявления о конфиденциальности и сведения о контактном лице, к которому можно обращаться по вопросам, касающимся этого заявления.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: directory-management
author: davidmu1
ms.openlocfilehash: 986f995458c56869d966c3c1baa2dc2f5df9aca1
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137671"
---
# <a name="privacyprofile-resource-type"></a><span data-ttu-id="ed0fc-103">Тип ресурса privacyProfile</span><span class="sxs-lookup"><span data-stu-id="ed0fc-103">privacyProfile resource type</span></span>

<span data-ttu-id="ed0fc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ed0fc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ed0fc-105">Представляет профиль конфиденциальности организации, который включает URL-адрес заявления о конфиденциальности и сведения о контактном лице, к которому можно обращаться по вопросам, касающимся этого заявления.</span><span class="sxs-lookup"><span data-stu-id="ed0fc-105">Represents a company's privacy profile, which includes a privacy statement URL and a contact person for questions regarding the privacy statement.</span></span>

## <a name="properties"></a><span data-ttu-id="ed0fc-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="ed0fc-106">Properties</span></span>
| <span data-ttu-id="ed0fc-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="ed0fc-107">Property</span></span>   | <span data-ttu-id="ed0fc-108">Тип</span><span class="sxs-lookup"><span data-stu-id="ed0fc-108">Type</span></span>|<span data-ttu-id="ed0fc-109">Описание</span><span class="sxs-lookup"><span data-stu-id="ed0fc-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ed0fc-110">contactEmail</span><span class="sxs-lookup"><span data-stu-id="ed0fc-110">contactEmail</span></span>|<span data-ttu-id="ed0fc-111">String</span><span class="sxs-lookup"><span data-stu-id="ed0fc-111">String</span></span>| <span data-ttu-id="ed0fc-112">Допустимый электронный адрес SMTP для контактного лица, к которому можно обращаться по вопросам, касающимся заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="ed0fc-112">A valid smtp email address for the privacy statement contact.</span></span> <span data-ttu-id="ed0fc-113">Не обязательное.</span><span class="sxs-lookup"><span data-stu-id="ed0fc-113">Not required.</span></span>|
|<span data-ttu-id="ed0fc-114">statementUrl</span><span class="sxs-lookup"><span data-stu-id="ed0fc-114">statementUrl</span></span>|<span data-ttu-id="ed0fc-115">String</span><span class="sxs-lookup"><span data-stu-id="ed0fc-115">String</span></span>| <span data-ttu-id="ed0fc-116">Допустимый формат URL-адреса, который начинается с http:// или https://.</span><span class="sxs-lookup"><span data-stu-id="ed0fc-116">A valid URL format that begins with http:// or https://.</span></span> <span data-ttu-id="ed0fc-117">Максимальная длина составляет 255 символов.</span><span class="sxs-lookup"><span data-stu-id="ed0fc-117">Maximum length is 255 characters.</span></span> <span data-ttu-id="ed0fc-118">URL-адрес заявления о конфиденциальности организации.</span><span class="sxs-lookup"><span data-stu-id="ed0fc-118">The URL that directs to the company's privacy statement.</span></span> <span data-ttu-id="ed0fc-119">Не обязательное.</span><span class="sxs-lookup"><span data-stu-id="ed0fc-119">Not required.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ed0fc-120">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="ed0fc-120">JSON representation</span></span>

<span data-ttu-id="ed0fc-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ed0fc-121">Here is a JSON representation of the resource</span></span>

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


