---
title: Тип ресурса Мфадетаил
description: 'Указывает сведения о MFA для определенного входа. Он включает способ проверки подлинности, используемый для входа в систему, а также сведения о проверке подлинности (например, Phone, SMS или голосовой почте). '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 15c15d3ec6db5acb16387a4b76501229167b0912
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522647"
---
# <a name="mfadetail-resource-type"></a><span data-ttu-id="e6429-104">Тип ресурса Мфадетаил</span><span class="sxs-lookup"><span data-stu-id="e6429-104">mfaDetail resource type</span></span>

<span data-ttu-id="e6429-105">Пространство имен: Microsoft. Graph указывает сведения о MFA для определенного входа.</span><span class="sxs-lookup"><span data-stu-id="e6429-105">Namespace: microsoft.graph Indicates MFA details for a specific sign-in.</span></span> <span data-ttu-id="e6429-106">Он включает способ проверки подлинности, используемый для входа в систему, а также сведения о проверке подлинности (например, Phone, SMS или голосовой почте).</span><span class="sxs-lookup"><span data-stu-id="e6429-106">It includes the authentication method used for signing in as well as auth details (for example: Phone, SMS or voicemail)</span></span> 



## <a name="properties"></a><span data-ttu-id="e6429-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="e6429-107">Properties</span></span>
| <span data-ttu-id="e6429-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="e6429-108">Property</span></span>     | <span data-ttu-id="e6429-109">Тип</span><span class="sxs-lookup"><span data-stu-id="e6429-109">Type</span></span>   |<span data-ttu-id="e6429-110">Описание</span><span class="sxs-lookup"><span data-stu-id="e6429-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e6429-111">аусдетаил</span><span class="sxs-lookup"><span data-stu-id="e6429-111">authDetail</span></span>|<span data-ttu-id="e6429-112">String</span><span class="sxs-lookup"><span data-stu-id="e6429-112">String</span></span>|<span data-ttu-id="e6429-113">Указывает сведения о проверке подлинности MFA для соответствующего действия при входе, если для MFA необходимо значение "Да".</span><span class="sxs-lookup"><span data-stu-id="e6429-113">Indicates the MFA auth detail for the corresponding Sign-in activity when the MFA Required is "Yes".</span></span>|
|<span data-ttu-id="e6429-114">аусмесод</span><span class="sxs-lookup"><span data-stu-id="e6429-114">authMethod</span></span>|<span data-ttu-id="e6429-115">String</span><span class="sxs-lookup"><span data-stu-id="e6429-115">String</span></span>|<span data-ttu-id="e6429-116">Указывает методы проверки подлинности MFA (SMS, Phone, приложение проверки подлинности — это часть значения) для соответствующего действия входа, если поле "обязательное MFA" имеет значение "Да".</span><span class="sxs-lookup"><span data-stu-id="e6429-116">Indicates the MFA Auth methods (SMS, Phone, Authenticator App are some of the value) for the corresponding sign-in activity when the MFA Required field is "Yes".</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e6429-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e6429-117">JSON representation</span></span>

<span data-ttu-id="e6429-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e6429-118">Here is a JSON representation of the resource.</span></span>

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
