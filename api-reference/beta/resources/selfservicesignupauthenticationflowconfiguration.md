---
title: Тип ресурса Селфсервицесигнупаусентикатионфловконфигуратион
description: Представляет конфигурации, связанные с регистрацией самостоятельной службы.
author: linkhp
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 8c75b3a90a7e9de01234bb53ed8346c40eef932f
ms.sourcegitcommit: b2e216de4a649606c961b3ed2aa3eb8a65f2355c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2020
ms.locfileid: "44556449"
---
# <a name="selfservicesignupauthenticationflowconfiguration-resource-type"></a><span data-ttu-id="751ad-103">Тип ресурса Селфсервицесигнупаусентикатионфловконфигуратион</span><span class="sxs-lookup"><span data-stu-id="751ad-103">selfServiceSignUpAuthenticationFlowConfiguration resource type</span></span>


<span data-ttu-id="751ad-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="751ad-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="751ad-105">Представляет конфигурации, связанные с самостоятельным входом.</span><span class="sxs-lookup"><span data-stu-id="751ad-105">Represents the configurations related to self-service sign up.</span></span>

## <a name="properties"></a><span data-ttu-id="751ad-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="751ad-106">Properties</span></span>
|<span data-ttu-id="751ad-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="751ad-107">Property</span></span>|<span data-ttu-id="751ad-108">Тип</span><span class="sxs-lookup"><span data-stu-id="751ad-108">Type</span></span>|<span data-ttu-id="751ad-109">Описание</span><span class="sxs-lookup"><span data-stu-id="751ad-109">Description</span></span>|
|:-------|:---|:----------|
|<span data-ttu-id="751ad-110">isEnabled</span><span class="sxs-lookup"><span data-stu-id="751ad-110">isEnabled</span></span>|<span data-ttu-id="751ad-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="751ad-111">Boolean</span></span>|<span data-ttu-id="751ad-112">Указывает, включен или отключен процесс самостоятельной регистрации для самостоятельных служб.</span><span class="sxs-lookup"><span data-stu-id="751ad-112">Indicates whether self-service sign-up flow is enabled or disabled.</span></span> <span data-ttu-id="751ad-113">Значение по умолчанию — `false`.</span><span class="sxs-lookup"><span data-stu-id="751ad-113">The default value is `false`.</span></span> <span data-ttu-id="751ad-114">Это свойство не является ключом.</span><span class="sxs-lookup"><span data-stu-id="751ad-114">This property is not a key.</span></span> <span data-ttu-id="751ad-115">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="751ad-115">Required.</span></span> |

## <a name="relationships"></a><span data-ttu-id="751ad-116">Связи</span><span class="sxs-lookup"><span data-stu-id="751ad-116">Relationships</span></span>
<span data-ttu-id="751ad-117">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="751ad-117">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="751ad-118">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="751ad-118">JSON representation</span></span>
<span data-ttu-id="751ad-119">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="751ad-119">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.selfServiceSignUpAuthenticationFlowConfiguration"
}
-->

``` json
{
  "isEnabled": "Boolean"
}
```
