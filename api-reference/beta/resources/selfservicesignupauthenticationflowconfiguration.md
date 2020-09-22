---
title: selfServiceSignUpAuthenticationFlowConfiguration resource type
description: Представляет конфигурации, связанные с самостоятельной регистрацией.
author: linkhp
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 658e27e4fe75424f4bd39cc6c3a76255e70c4d92
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47988809"
---
# <a name="selfservicesignupauthenticationflowconfiguration-resource-type"></a><span data-ttu-id="d271b-103">selfServiceSignUpAuthenticationFlowConfiguration resource type</span><span class="sxs-lookup"><span data-stu-id="d271b-103">selfServiceSignUpAuthenticationFlowConfiguration resource type</span></span>


<span data-ttu-id="d271b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d271b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d271b-105">Представляет конфигурации, связанные с самостоятельной регистрацией.</span><span class="sxs-lookup"><span data-stu-id="d271b-105">Represents the configurations related to self-service sign up.</span></span>

## <a name="properties"></a><span data-ttu-id="d271b-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="d271b-106">Properties</span></span>
|<span data-ttu-id="d271b-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="d271b-107">Property</span></span>|<span data-ttu-id="d271b-108">Тип</span><span class="sxs-lookup"><span data-stu-id="d271b-108">Type</span></span>|<span data-ttu-id="d271b-109">Описание</span><span class="sxs-lookup"><span data-stu-id="d271b-109">Description</span></span>|
|:-------|:---|:----------|
|<span data-ttu-id="d271b-110">isEnabled</span><span class="sxs-lookup"><span data-stu-id="d271b-110">isEnabled</span></span>|<span data-ttu-id="d271b-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="d271b-111">Boolean</span></span>|<span data-ttu-id="d271b-112">Указывает, включена или выключена ли самостоятельная регистрация.</span><span class="sxs-lookup"><span data-stu-id="d271b-112">Indicates whether self-service sign-up flow is enabled or disabled.</span></span> <span data-ttu-id="d271b-113">Значение по умолчанию — `false`.</span><span class="sxs-lookup"><span data-stu-id="d271b-113">The default value is `false`.</span></span> <span data-ttu-id="d271b-114">Это свойство не является ключевым.</span><span class="sxs-lookup"><span data-stu-id="d271b-114">This property is not a key.</span></span> <span data-ttu-id="d271b-115">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d271b-115">Required.</span></span> |

## <a name="relationships"></a><span data-ttu-id="d271b-116">Связи</span><span class="sxs-lookup"><span data-stu-id="d271b-116">Relationships</span></span>
<span data-ttu-id="d271b-117">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="d271b-117">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d271b-118">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="d271b-118">JSON representation</span></span>
<span data-ttu-id="d271b-119">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d271b-119">The following is a JSON representation of the resource.</span></span>
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


