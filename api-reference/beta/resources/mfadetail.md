---
title: тип ресурса mfaDetail
description: 'Указывает сведения MFA для определенного входного знака. Он включает метод проверки подлинности, используемый для регистрации, а также сведения об auth (например: телефон, SMS или голосовая почта) '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: identity-and-access-reports
author: besiler
ms.openlocfilehash: b3cd2392b9591cfb5465f2f269db547cd37754ea
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/12/2021
ms.locfileid: "50759799"
---
# <a name="mfadetail-resource-type"></a><span data-ttu-id="35e65-104">тип ресурса mfaDetail</span><span class="sxs-lookup"><span data-stu-id="35e65-104">mfaDetail resource type</span></span>

<span data-ttu-id="35e65-105">Пространство имен: microsoft.graph указывает сведения MFA для определенного входного знака.</span><span class="sxs-lookup"><span data-stu-id="35e65-105">Namespace: microsoft.graph Indicates MFA details for a specific sign-in.</span></span> <span data-ttu-id="35e65-106">Он включает метод проверки подлинности, используемый для регистрации, а также сведения об auth (например: телефон, SMS или голосовая почта)</span><span class="sxs-lookup"><span data-stu-id="35e65-106">It includes the authentication method used for signing in as well as auth details (for example: Phone, SMS or voicemail)</span></span>



## <a name="properties"></a><span data-ttu-id="35e65-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="35e65-107">Properties</span></span>
| <span data-ttu-id="35e65-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="35e65-108">Property</span></span>     | <span data-ttu-id="35e65-109">Тип</span><span class="sxs-lookup"><span data-stu-id="35e65-109">Type</span></span>   |<span data-ttu-id="35e65-110">Описание</span><span class="sxs-lookup"><span data-stu-id="35e65-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="35e65-111">authDetail</span><span class="sxs-lookup"><span data-stu-id="35e65-111">authDetail</span></span>|<span data-ttu-id="35e65-112">String</span><span class="sxs-lookup"><span data-stu-id="35e65-112">String</span></span>|<span data-ttu-id="35e65-113">Указывает подробную информацию об auth MFA для соответствующей активности регистрации, когда требуется MFA является "Да".</span><span class="sxs-lookup"><span data-stu-id="35e65-113">Indicates the MFA auth detail for the corresponding Sign-in activity when the MFA Required is "Yes".</span></span>|
|<span data-ttu-id="35e65-114">authMethod</span><span class="sxs-lookup"><span data-stu-id="35e65-114">authMethod</span></span>|<span data-ttu-id="35e65-115">String</span><span class="sxs-lookup"><span data-stu-id="35e65-115">String</span></span>|<span data-ttu-id="35e65-116">Указывает, что методы auth MFA (SMS, Phone, Authenticator App являются некоторыми из значений) для соответствующей активности входных данных, когда поле MFA Обязательное "Да".</span><span class="sxs-lookup"><span data-stu-id="35e65-116">Indicates the MFA Auth methods (SMS, Phone, Authenticator App are some of the value) for the corresponding sign-in activity when the MFA Required field is "Yes".</span></span>|

## <a name="json-representation"></a><span data-ttu-id="35e65-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="35e65-117">JSON representation</span></span>

<span data-ttu-id="35e65-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="35e65-118">Here is a JSON representation of the resource.</span></span>

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


