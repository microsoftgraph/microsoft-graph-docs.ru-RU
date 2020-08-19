---
title: Тип ресурса Мфадетаил
description: 'Указывает сведения о MFA для определенного входа. Он включает способ проверки подлинности, используемый для входа в систему, а также сведения о проверке подлинности (например, Phone, SMS или голосовой почте). '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: khotz
ms.openlocfilehash: f58736d890bc530239be413aec9a6920c64856ee
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46809364"
---
# <a name="mfadetail-resource-type"></a><span data-ttu-id="6c4a8-104">Тип ресурса Мфадетаил</span><span class="sxs-lookup"><span data-stu-id="6c4a8-104">mfaDetail resource type</span></span>

<span data-ttu-id="6c4a8-105">Пространство имен: Microsoft. Graph указывает сведения о MFA для определенного входа.</span><span class="sxs-lookup"><span data-stu-id="6c4a8-105">Namespace: microsoft.graph Indicates MFA details for a specific sign-in.</span></span> <span data-ttu-id="6c4a8-106">Он включает способ проверки подлинности, используемый для входа в систему, а также сведения о проверке подлинности (например, Phone, SMS или голосовой почте).</span><span class="sxs-lookup"><span data-stu-id="6c4a8-106">It includes the authentication method used for signing in as well as auth details (for example: Phone, SMS or voicemail)</span></span>



## <a name="properties"></a><span data-ttu-id="6c4a8-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="6c4a8-107">Properties</span></span>
| <span data-ttu-id="6c4a8-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="6c4a8-108">Property</span></span>     | <span data-ttu-id="6c4a8-109">Тип</span><span class="sxs-lookup"><span data-stu-id="6c4a8-109">Type</span></span>   |<span data-ttu-id="6c4a8-110">Описание</span><span class="sxs-lookup"><span data-stu-id="6c4a8-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6c4a8-111">аусдетаил</span><span class="sxs-lookup"><span data-stu-id="6c4a8-111">authDetail</span></span>|<span data-ttu-id="6c4a8-112">String</span><span class="sxs-lookup"><span data-stu-id="6c4a8-112">String</span></span>|<span data-ttu-id="6c4a8-113">Указывает сведения о проверке подлинности MFA для соответствующего действия при входе, если для MFA необходимо значение "Да".</span><span class="sxs-lookup"><span data-stu-id="6c4a8-113">Indicates the MFA auth detail for the corresponding Sign-in activity when the MFA Required is "Yes".</span></span>|
|<span data-ttu-id="6c4a8-114">аусмесод</span><span class="sxs-lookup"><span data-stu-id="6c4a8-114">authMethod</span></span>|<span data-ttu-id="6c4a8-115">String</span><span class="sxs-lookup"><span data-stu-id="6c4a8-115">String</span></span>|<span data-ttu-id="6c4a8-116">Указывает методы проверки подлинности MFA (SMS, Phone, приложение проверки подлинности — это часть значения) для соответствующего действия входа, если поле "обязательное MFA" имеет значение "Да".</span><span class="sxs-lookup"><span data-stu-id="6c4a8-116">Indicates the MFA Auth methods (SMS, Phone, Authenticator App are some of the value) for the corresponding sign-in activity when the MFA Required field is "Yes".</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6c4a8-117">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="6c4a8-117">JSON representation</span></span>

<span data-ttu-id="6c4a8-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6c4a8-118">Here is a JSON representation of the resource.</span></span>

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
