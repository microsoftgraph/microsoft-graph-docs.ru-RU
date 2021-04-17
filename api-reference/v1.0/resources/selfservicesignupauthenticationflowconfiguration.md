---
title: selfServiceSignUpAuthenticationFlowConfiguration resource type
description: Представляет конфигурации, связанные с самостоятельной регистрацией.
author: linkhp
localization_priority: Priority
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: a235c9e9869b3e0b0c36b0369ae6163083b3cf20
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/17/2021
ms.locfileid: "51883314"
---
# <a name="selfservicesignupauthenticationflowconfiguration-resource-type"></a><span data-ttu-id="37ccd-103">selfServiceSignUpAuthenticationFlowConfiguration resource type</span><span class="sxs-lookup"><span data-stu-id="37ccd-103">selfServiceSignUpAuthenticationFlowConfiguration resource type</span></span>

<span data-ttu-id="37ccd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="37ccd-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="37ccd-105">Представляет конфигурации, связанные с самостоятельной регистрацией.</span><span class="sxs-lookup"><span data-stu-id="37ccd-105">Represents the configurations related to self-service sign-up.</span></span>

## <a name="properties"></a><span data-ttu-id="37ccd-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="37ccd-106">Properties</span></span>

|<span data-ttu-id="37ccd-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="37ccd-107">Property</span></span>|<span data-ttu-id="37ccd-108">Тип</span><span class="sxs-lookup"><span data-stu-id="37ccd-108">Type</span></span>|<span data-ttu-id="37ccd-109">Описание</span><span class="sxs-lookup"><span data-stu-id="37ccd-109">Description</span></span>|
|:-------|:---|:----------|
|<span data-ttu-id="37ccd-110">isEnabled</span><span class="sxs-lookup"><span data-stu-id="37ccd-110">isEnabled</span></span>|<span data-ttu-id="37ccd-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="37ccd-111">Boolean</span></span>|<span data-ttu-id="37ccd-112">Указывает, включена или выключена ли самостоятельная регистрация.</span><span class="sxs-lookup"><span data-stu-id="37ccd-112">Indicates whether self-service sign-up flow is enabled or disabled.</span></span> <span data-ttu-id="37ccd-113">Значение по умолчанию — `false`.</span><span class="sxs-lookup"><span data-stu-id="37ccd-113">The default value is `false`.</span></span> <span data-ttu-id="37ccd-114">Это свойство не является ключевым.</span><span class="sxs-lookup"><span data-stu-id="37ccd-114">This property is not a key.</span></span> <span data-ttu-id="37ccd-115">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="37ccd-115">Required.</span></span> |

## <a name="relationships"></a><span data-ttu-id="37ccd-116">Связи</span><span class="sxs-lookup"><span data-stu-id="37ccd-116">Relationships</span></span>

<span data-ttu-id="37ccd-117">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="37ccd-117">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="37ccd-118">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="37ccd-118">JSON representation</span></span>

<span data-ttu-id="37ccd-119">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="37ccd-119">The following is a JSON representation of the resource.</span></span>
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
