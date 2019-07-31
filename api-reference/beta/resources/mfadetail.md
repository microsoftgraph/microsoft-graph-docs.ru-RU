---
title: Тип ресурса Мфадетаил
description: 'Указывает сведения о MFA для определенного входа. Он включает способ проверки подлинности, используемый для входа в систему, а также сведения о проверке подлинности (например, Phone, SMS или голосовой почте). '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 3f38fae4d0360386592f956bee05d55738ad6910
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009666"
---
# <a name="mfadetail-resource-type"></a><span data-ttu-id="91b09-104">Тип ресурса Мфадетаил</span><span class="sxs-lookup"><span data-stu-id="91b09-104">mfaDetail resource type</span></span>
<span data-ttu-id="91b09-105">Указывает сведения о MFA для определенного входа.</span><span class="sxs-lookup"><span data-stu-id="91b09-105">Indicates MFA details for a specific sign-in.</span></span> <span data-ttu-id="91b09-106">Он включает способ проверки подлинности, используемый для входа в систему, а также сведения о проверке подлинности (например, Phone, SMS или голосовой почте).</span><span class="sxs-lookup"><span data-stu-id="91b09-106">It includes the authentication method used for signing in as well as auth details (for example: Phone, SMS or voicemail)</span></span> 



## <a name="properties"></a><span data-ttu-id="91b09-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="91b09-107">Properties</span></span>
| <span data-ttu-id="91b09-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="91b09-108">Property</span></span>     | <span data-ttu-id="91b09-109">Тип</span><span class="sxs-lookup"><span data-stu-id="91b09-109">Type</span></span>   |<span data-ttu-id="91b09-110">Описание</span><span class="sxs-lookup"><span data-stu-id="91b09-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="91b09-111">Аусдетаил</span><span class="sxs-lookup"><span data-stu-id="91b09-111">authDetail</span></span>|<span data-ttu-id="91b09-112">String</span><span class="sxs-lookup"><span data-stu-id="91b09-112">String</span></span>|<span data-ttu-id="91b09-113">Указывает сведения о проверке подлинности MFA для соответствующего действия при входе, если для MFA необходимо значение "Да".</span><span class="sxs-lookup"><span data-stu-id="91b09-113">Indicates the MFA auth detail for the corresponding Sign-in activity when the MFA Required is "Yes".</span></span>|
|<span data-ttu-id="91b09-114">Аусмесод</span><span class="sxs-lookup"><span data-stu-id="91b09-114">authMethod</span></span>|<span data-ttu-id="91b09-115">String</span><span class="sxs-lookup"><span data-stu-id="91b09-115">String</span></span>|<span data-ttu-id="91b09-116">Указывает методы проверки подлинности MFA (SMS, Phone, приложение проверки подлинности — это часть значения) для соответствующего действия входа, если поле "обязательное MFA" имеет значение "Да".</span><span class="sxs-lookup"><span data-stu-id="91b09-116">Indicates the MFA Auth methods (SMS, Phone, Authenticator App are some of the value) for the corresponding sign-in activity when the MFA Required field is "Yes".</span></span>|

## <a name="json-representation"></a><span data-ttu-id="91b09-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="91b09-117">JSON representation</span></span>

<span data-ttu-id="91b09-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="91b09-118">Here is a JSON representation of the resource.</span></span>

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
