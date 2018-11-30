---
title: Тип перечисления binaryManagementConditionExpressionOperatorType
description: Поддерживаемые двоичные операторы для управления условным выражением.
ms.openlocfilehash: e1f58715f4e900c30a52bbe7a9db01e45a081d09
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27082366"
---
# <a name="binarymanagementconditionexpressionoperatortype-enum-type"></a><span data-ttu-id="ddb40-103">Тип перечисления binaryManagementConditionExpressionOperatorType</span><span class="sxs-lookup"><span data-stu-id="ddb40-103">binaryManagementConditionExpressionOperatorType enum type</span></span>

> <span data-ttu-id="ddb40-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ddb40-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ddb40-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ddb40-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ddb40-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="ddb40-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ddb40-107">Поддерживаемые двоичные операторы для управления условным выражением.</span><span class="sxs-lookup"><span data-stu-id="ddb40-107">Supported binary operators for management condition expressions.</span></span>
## <a name="members"></a><span data-ttu-id="ddb40-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="ddb40-108">Members</span></span>
|<span data-ttu-id="ddb40-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="ddb40-109">Member</span></span>|<span data-ttu-id="ddb40-110">Значение</span><span class="sxs-lookup"><span data-stu-id="ddb40-110">Value</span></span>|<span data-ttu-id="ddb40-111">Description</span><span class="sxs-lookup"><span data-stu-id="ddb40-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ddb40-112">или</span><span class="sxs-lookup"><span data-stu-id="ddb40-112">or</span></span>|<span data-ttu-id="ddb40-113">0</span><span class="sxs-lookup"><span data-stu-id="ddb40-113">0</span></span>|<span data-ttu-id="ddb40-114">Вычисляется набора операндов true только в том случае, если один или несколько операндов имеет значение true.</span><span class="sxs-lookup"><span data-stu-id="ddb40-114">Evaluates a set of operands as true if and only if one or more of its operands is true.</span></span>|
|<span data-ttu-id="ddb40-115">и</span><span class="sxs-lookup"><span data-stu-id="ddb40-115">and</span></span>|<span data-ttu-id="ddb40-116">1</span><span class="sxs-lookup"><span data-stu-id="ddb40-116">1</span></span>|<span data-ttu-id="ddb40-117">Вычисляется набора операндов true только в том случае, если выполняются все операндов.</span><span class="sxs-lookup"><span data-stu-id="ddb40-117">Evaluates a set of operands as true if and only if all of its operands are true.</span></span>|





