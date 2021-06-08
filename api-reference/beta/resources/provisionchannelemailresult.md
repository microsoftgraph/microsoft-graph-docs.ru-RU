---
title: тип ресурса provisionChannelEmailResult
description: Представляет результат операции по подготовка электронной почты канала.
author: anandab-msft
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: ac32dd0db4877dc01a13536689d414b0dcc1175f
ms.sourcegitcommit: a2d81138de2a0404e611fbb535679199477ef3d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/08/2021
ms.locfileid: "52813253"
---
# <a name="provisionchannelemailresult-resource-type"></a><span data-ttu-id="9f7fd-103">тип ресурса provisionChannelEmailResult</span><span class="sxs-lookup"><span data-stu-id="9f7fd-103">provisionChannelEmailResult resource type</span></span>

<span data-ttu-id="9f7fd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9f7fd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9f7fd-105">Представляет адрес электронной [почты, который был предусмотрен](..\api\channel-provisionemail.md) для [канала.](channel.md)</span><span class="sxs-lookup"><span data-stu-id="9f7fd-105">Represents the email address [provisioned](..\api\channel-provisionemail.md) for a [channel](channel.md).</span></span>

## <a name="properties"></a><span data-ttu-id="9f7fd-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="9f7fd-106">Properties</span></span>
| <span data-ttu-id="9f7fd-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="9f7fd-107">Property</span></span> | <span data-ttu-id="9f7fd-108">Тип</span><span class="sxs-lookup"><span data-stu-id="9f7fd-108">Type</span></span>   | <span data-ttu-id="9f7fd-109">Описание</span><span class="sxs-lookup"><span data-stu-id="9f7fd-109">Description</span></span>                               |
| :------- | :----- | :---------------------------------------- |
| <span data-ttu-id="9f7fd-110">email</span><span class="sxs-lookup"><span data-stu-id="9f7fd-110">email</span></span>    | <span data-ttu-id="9f7fd-111">String</span><span class="sxs-lookup"><span data-stu-id="9f7fd-111">String</span></span> | <span data-ttu-id="9f7fd-112">Представляет предварительный адрес электронной почты.</span><span class="sxs-lookup"><span data-stu-id="9f7fd-112">Represents the provisioned email address.</span></span> |

## <a name="relationships"></a><span data-ttu-id="9f7fd-113">Связи</span><span class="sxs-lookup"><span data-stu-id="9f7fd-113">Relationships</span></span>
<span data-ttu-id="9f7fd-114">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="9f7fd-114">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9f7fd-115">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="9f7fd-115">JSON representation</span></span>
<span data-ttu-id="9f7fd-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9f7fd-116">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.provisionChannelEmailResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.provisionChannelEmailResult",
  "email": "String"
}
```
