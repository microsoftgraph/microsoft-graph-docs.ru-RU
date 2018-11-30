---
title: Тип ресурса mfaDetail
description: 'Указывает сведения о многофакторной проверкой Подлинности для конкретного учетное. Он содержит метод проверки подлинности, используемый для подписи, а также сведения о проверкой подлинности на основе (например: телефон, SMS или голосовая почта) '
ms.openlocfilehash: a377c8648ebc8a6e3eb10fb6b0b87df066f8f2cc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078087"
---
# <a name="mfadetail-resource-type"></a><span data-ttu-id="8afdc-104">Тип ресурса mfaDetail</span><span class="sxs-lookup"><span data-stu-id="8afdc-104">mfaDetail resource type</span></span>
<span data-ttu-id="8afdc-105">Указывает сведения о многофакторной проверкой Подлинности для конкретного учетное.</span><span class="sxs-lookup"><span data-stu-id="8afdc-105">Indicates MFA details for a specific sign-in.</span></span> <span data-ttu-id="8afdc-106">Он содержит метод проверки подлинности, используемый для подписи, а также сведения о проверкой подлинности на основе (например: телефон, SMS или голосовая почта)</span><span class="sxs-lookup"><span data-stu-id="8afdc-106">It includes the authentication method used for signing in as well as auth details (for example: Phone, SMS or voicemail)</span></span> 



## <a name="properties"></a><span data-ttu-id="8afdc-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="8afdc-107">Properties</span></span>
| <span data-ttu-id="8afdc-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="8afdc-108">Property</span></span>     | <span data-ttu-id="8afdc-109">Тип</span><span class="sxs-lookup"><span data-stu-id="8afdc-109">Type</span></span>   |<span data-ttu-id="8afdc-110">Description</span><span class="sxs-lookup"><span data-stu-id="8afdc-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8afdc-111">authDetail</span><span class="sxs-lookup"><span data-stu-id="8afdc-111">authDetail</span></span>|<span data-ttu-id="8afdc-112">String</span><span class="sxs-lookup"><span data-stu-id="8afdc-112">String</span></span>|<span data-ttu-id="8afdc-113">Указывает детализации проверкой подлинности на основе многофакторной проверкой Подлинности для соответствующего действия входа при многофакторной проверкой Подлинности, который требуется — «Да».</span><span class="sxs-lookup"><span data-stu-id="8afdc-113">Indicates the MFA auth detail for the corresponding Sign-in activity when the MFA Required is "Yes".</span></span>|
|<span data-ttu-id="8afdc-114">метод проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="8afdc-114">authMethod</span></span>|<span data-ttu-id="8afdc-115">String</span><span class="sxs-lookup"><span data-stu-id="8afdc-115">String</span></span>|<span data-ttu-id="8afdc-116">Указывает многофакторной проверкой Подлинности методов проверки подлинности (SMS, телефонную связь, проверки подлинности приложения представлены некоторые значения) для соответствующего действия входа при многофакторной проверкой Подлинности необходимые поля — «Да».</span><span class="sxs-lookup"><span data-stu-id="8afdc-116">Indicates the MFA Auth methods (SMS, Phone, Authenticator App are some of the value) for the corresponding sign-in activity when the MFA Required field is "Yes".</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8afdc-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8afdc-117">JSON representation</span></span>

<span data-ttu-id="8afdc-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8afdc-118">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.mfaDetail"
}-->

```json
{
  "authDetail": "String",
  "authMethod": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mfaDetail resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->