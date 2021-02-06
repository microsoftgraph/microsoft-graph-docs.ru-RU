---
title: Тип ресурса userRegistrationMethodCount
description: Количество пользователей, зарегистрированных для метода проверки подлинности.
author: danielwood95
localization_priority: Normal
ms.prod: reports
doc_type: resourcePageType
ms.openlocfilehash: 8e4c19c48771ccd0bd1dd1f1a4b049334266834a
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132939"
---
# <a name="userregistrationmethodcount-resource-type"></a><span data-ttu-id="79013-103">Тип ресурса userRegistrationMethodCount</span><span class="sxs-lookup"><span data-stu-id="79013-103">userRegistrationMethodCount resource type</span></span>

<span data-ttu-id="79013-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="79013-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="79013-105">Количество пользователей, зарегистрированных для метода проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="79013-105">Number of users registered for an authentication method.</span></span>

## <a name="properties"></a><span data-ttu-id="79013-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="79013-106">Properties</span></span>
|<span data-ttu-id="79013-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="79013-107">Property</span></span>|<span data-ttu-id="79013-108">Тип</span><span class="sxs-lookup"><span data-stu-id="79013-108">Type</span></span>|<span data-ttu-id="79013-109">Описание</span><span class="sxs-lookup"><span data-stu-id="79013-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="79013-110">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="79013-110">authenticationMethod</span></span>|<span data-ttu-id="79013-111">Строка</span><span class="sxs-lookup"><span data-stu-id="79013-111">String</span></span>|<span data-ttu-id="79013-112">Имя метода проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="79013-112">Name of authentication method.</span></span>|
|<span data-ttu-id="79013-113">userCount</span><span class="sxs-lookup"><span data-stu-id="79013-113">userCount</span></span>|<span data-ttu-id="79013-114">Int64</span><span class="sxs-lookup"><span data-stu-id="79013-114">Int64</span></span>|<span data-ttu-id="79013-115">Количество зарегистрированных пользователей.</span><span class="sxs-lookup"><span data-stu-id="79013-115">Number of users registered.</span></span>|

## <a name="relationships"></a><span data-ttu-id="79013-116">Связи</span><span class="sxs-lookup"><span data-stu-id="79013-116">Relationships</span></span>
<span data-ttu-id="79013-117">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="79013-117">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="79013-118">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="79013-118">JSON representation</span></span>
<span data-ttu-id="79013-119">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="79013-119">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userRegistrationMethodCount"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userRegistrationMethodCount",
  "authenticationMethod": "String",
  "userCount": "Integer"
}
```
