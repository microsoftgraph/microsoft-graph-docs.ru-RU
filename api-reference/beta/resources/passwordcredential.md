---
title: Тип ресурса Пассвордкредентиал
description: Содержит учетные данные пароля, связанные с приложением или субъектом службы. Свойство **пассвордкредентиалс** объекта servicePrincipal и сущности приложения является коллекцией **пассвордкредентиал**.
localization_priority: Normal
ms.openlocfilehash: 900bfb8a5828d636dfa1f1abfd0348ceb4aee143
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32568469"
---
# <a name="passwordcredential-resource-type"></a><span data-ttu-id="89397-104">Тип ресурса Пассвордкредентиал</span><span class="sxs-lookup"><span data-stu-id="89397-104">passwordCredential resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="89397-105">Содержит учетные данные пароля, связанные с приложением или субъектом службы.</span><span class="sxs-lookup"><span data-stu-id="89397-105">Contains a password credential associated with an application or a service principal.</span></span> <span data-ttu-id="89397-106">Свойство **пассвордкредентиалс** объекта [servicePrincipal](serviceprincipal.md) и сущности [приложения](application.md) является коллекцией **пассвордкредентиал**.</span><span class="sxs-lookup"><span data-stu-id="89397-106">The **passwordCredentials** property of the [servicePrincipal](serviceprincipal.md) entity and of the [application](application.md) entity is a collection of **passwordCredential**.</span></span>


## <a name="json-representation"></a><span data-ttu-id="89397-107">Описание в формате JSON</span><span class="sxs-lookup"><span data-stu-id="89397-107">JSON representation</span></span>

<span data-ttu-id="89397-108">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="89397-108">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.passwordCredential"
}-->

```json
{
  "customKeyIdentifier": "binary",
  "endDateTime": "String (timestamp)",
  "keyId": "guid",
  "startDateTime": "String (timestamp)",
  "secretText": "string",
  "hint": "string"
}

```
## <a name="properties"></a><span data-ttu-id="89397-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="89397-109">Properties</span></span>
| <span data-ttu-id="89397-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="89397-110">Property</span></span>     | <span data-ttu-id="89397-111">Тип</span><span class="sxs-lookup"><span data-stu-id="89397-111">Type</span></span>   |<span data-ttu-id="89397-112">Описание</span><span class="sxs-lookup"><span data-stu-id="89397-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="89397-113">Кустомкэйидентифиер</span><span class="sxs-lookup"><span data-stu-id="89397-113">customKeyIdentifier</span></span>|<span data-ttu-id="89397-114">Двоичный</span><span class="sxs-lookup"><span data-stu-id="89397-114">Binary</span></span>|            |
|<span data-ttu-id="89397-115">endDateTime</span><span class="sxs-lookup"><span data-stu-id="89397-115">endDateTime</span></span>|<span data-ttu-id="89397-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="89397-116">DateTimeOffset</span></span>|<span data-ttu-id="89397-117">Дата и время истечения срока действия пароля. Тип timestamp представляет сведения о дате и времени с использованием формата ISO 8601 и всегда задается в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="89397-117">The date and time at which the password expires.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="89397-118">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="89397-118">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="89397-119">Него значение KeyID</span><span class="sxs-lookup"><span data-stu-id="89397-119">keyId</span></span>|<span data-ttu-id="89397-120">Guid</span><span class="sxs-lookup"><span data-stu-id="89397-120">Guid</span></span>|            |
|<span data-ttu-id="89397-121">startDateTime</span><span class="sxs-lookup"><span data-stu-id="89397-121">startDateTime</span></span>|<span data-ttu-id="89397-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="89397-122">DateTimeOffset</span></span>|<span data-ttu-id="89397-123">Дата и время, когда пароль становится действительным. Тип timestamp представляет сведения о дате и времени с использованием формата ISO 8601 и всегда задается в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="89397-123">The date and time at which the password becomes valid.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="89397-124">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="89397-124">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="89397-125">Секреттекст</span><span class="sxs-lookup"><span data-stu-id="89397-125">secretText</span></span>|<span data-ttu-id="89397-126">String</span><span class="sxs-lookup"><span data-stu-id="89397-126">String</span></span>| <span data-ttu-id="89397-127">Пароли должны иметь длину 16-64 символов</span><span class="sxs-lookup"><span data-stu-id="89397-127">The passwords must be 16-64 characters in length</span></span> |
|<span data-ttu-id="89397-128">сказок</span><span class="sxs-lookup"><span data-stu-id="89397-128">hint</span></span>|<span data-ttu-id="89397-129">String</span><span class="sxs-lookup"><span data-stu-id="89397-129">String</span></span>|  |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "passwordCredential resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
