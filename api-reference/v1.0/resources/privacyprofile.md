---
title: Тип ресурса privacyProfile
description: Представляет профиль конфиденциальности организации, который включает URL-адрес заявления о конфиденциальности и сведения о контактном лице, к которому можно обращаться по вопросам, касающимся этого заявления.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 09c3b8ad246bb8c653f31bfebda6013d8519007c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533951"
---
# <a name="privacyprofile-resource-type"></a><span data-ttu-id="41e20-103">Тип ресурса privacyProfile</span><span class="sxs-lookup"><span data-stu-id="41e20-103">privacyProfile resource type</span></span>

<span data-ttu-id="41e20-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="41e20-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="41e20-105">Представляет профиль конфиденциальности организации, который включает URL-адрес заявления о конфиденциальности и сведения о контактном лице, к которому можно обращаться по вопросам, касающимся этого заявления.</span><span class="sxs-lookup"><span data-stu-id="41e20-105">Represents a company's privacy profile, which includes a privacy statement URL and a contact person for questions regarding the privacy statement.</span></span>

## <a name="properties"></a><span data-ttu-id="41e20-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="41e20-106">Properties</span></span>
| <span data-ttu-id="41e20-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="41e20-107">Property</span></span>   | <span data-ttu-id="41e20-108">Тип</span><span class="sxs-lookup"><span data-stu-id="41e20-108">Type</span></span>|<span data-ttu-id="41e20-109">Описание</span><span class="sxs-lookup"><span data-stu-id="41e20-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="41e20-110">contactEmail</span><span class="sxs-lookup"><span data-stu-id="41e20-110">contactEmail</span></span>|<span data-ttu-id="41e20-111">String</span><span class="sxs-lookup"><span data-stu-id="41e20-111">String</span></span>| <span data-ttu-id="41e20-112">Допустимый электронный адрес SMTP для контактного лица, к которому можно обращаться по вопросам, касающимся заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="41e20-112">A valid smtp email address for the privacy statement contact.</span></span> <span data-ttu-id="41e20-113">Не требуется.</span><span class="sxs-lookup"><span data-stu-id="41e20-113">Not required.</span></span>|
|<span data-ttu-id="41e20-114">statementUrl</span><span class="sxs-lookup"><span data-stu-id="41e20-114">statementUrl</span></span>|<span data-ttu-id="41e20-115">String</span><span class="sxs-lookup"><span data-stu-id="41e20-115">String</span></span>| <span data-ttu-id="41e20-116">Допустимый формат URL-адреса, который начинается с http:// или https://.</span><span class="sxs-lookup"><span data-stu-id="41e20-116">A valid URL format that begins with http:// or https://.</span></span> <span data-ttu-id="41e20-117">Максимальная длина составляет 255 символов.</span><span class="sxs-lookup"><span data-stu-id="41e20-117">Maximum length is 255 characters.</span></span> <span data-ttu-id="41e20-118">URL-адрес заявления о конфиденциальности организации.</span><span class="sxs-lookup"><span data-stu-id="41e20-118">The URL that directs to the company's privacy statement.</span></span> <span data-ttu-id="41e20-119">Не обязательное.</span><span class="sxs-lookup"><span data-stu-id="41e20-119">Not required.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="41e20-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="41e20-120">JSON representation</span></span>

<span data-ttu-id="41e20-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="41e20-121">Here is a JSON representation of the resource</span></span>

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
