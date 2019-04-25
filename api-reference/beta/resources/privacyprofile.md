---
title: Тип ресурса privacyProfile
description: Представляет профиль конфиденциальности организации, который включает URL-адрес заявления о конфиденциальности и сведения о контактном лице, к которому можно обращаться по вопросам, касающимся этого заявления.
localization_priority: Normal
ms.openlocfilehash: 9c110cbdb8a456b43936d3b56db5d4563686ed6e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563612"
---
# <a name="privacyprofile-resource-type"></a><span data-ttu-id="840b4-103">Тип ресурса privacyProfile</span><span class="sxs-lookup"><span data-stu-id="840b4-103">privacyProfile resource type</span></span>

<span data-ttu-id="840b4-104">Представляет профиль конфиденциальности организации, который включает URL-адрес заявления о конфиденциальности и сведения о контактном лице, к которому можно обращаться по вопросам, касающимся этого заявления.</span><span class="sxs-lookup"><span data-stu-id="840b4-104">Represents a company's privacy profile, which includes a privacy statement URL and a contact person for questions regarding the privacy statement.</span></span>

## <a name="properties"></a><span data-ttu-id="840b4-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="840b4-105">Properties</span></span>
| <span data-ttu-id="840b4-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="840b4-106">Property</span></span>   | <span data-ttu-id="840b4-107">Тип</span><span class="sxs-lookup"><span data-stu-id="840b4-107">Type</span></span>|<span data-ttu-id="840b4-108">Описание</span><span class="sxs-lookup"><span data-stu-id="840b4-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="840b4-109">contactEmail</span><span class="sxs-lookup"><span data-stu-id="840b4-109">contactEmail</span></span>|<span data-ttu-id="840b4-110">String</span><span class="sxs-lookup"><span data-stu-id="840b4-110">String</span></span>| <span data-ttu-id="840b4-111">Допустимый электронный адрес SMTP для контактного лица, к которому можно обращаться по вопросам, касающимся заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="840b4-111">A valid smtp email address for the privacy statement contact.</span></span> <span data-ttu-id="840b4-112">Не требуется.</span><span class="sxs-lookup"><span data-stu-id="840b4-112">Not required.</span></span>|
|<span data-ttu-id="840b4-113">statementUrl</span><span class="sxs-lookup"><span data-stu-id="840b4-113">statementUrl</span></span>|<span data-ttu-id="840b4-114">String</span><span class="sxs-lookup"><span data-stu-id="840b4-114">String</span></span>| <span data-ttu-id="840b4-115">Допустимый формат URL-адреса, который начинается с http:// или https://.</span><span class="sxs-lookup"><span data-stu-id="840b4-115">A valid URL format that begins with http:// or https://.</span></span> <span data-ttu-id="840b4-116">Максимальная длина составляет 255 символов.</span><span class="sxs-lookup"><span data-stu-id="840b4-116">Maximum length is 255 characters.</span></span> <span data-ttu-id="840b4-117">URL-адрес заявления о конфиденциальности организации.</span><span class="sxs-lookup"><span data-stu-id="840b4-117">The URL that directs to the company's privacy statement.</span></span> <span data-ttu-id="840b4-118">Не обязательное.</span><span class="sxs-lookup"><span data-stu-id="840b4-118">Not required.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="840b4-119">Описание в формате JSON</span><span class="sxs-lookup"><span data-stu-id="840b4-119">JSON representation</span></span>

<span data-ttu-id="840b4-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="840b4-120">Here is a JSON representation of the resource</span></span>

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
