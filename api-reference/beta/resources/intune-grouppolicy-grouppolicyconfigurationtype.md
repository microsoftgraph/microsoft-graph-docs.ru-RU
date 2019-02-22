---
title: тип перечисления Граупполициконфигуратионтипе
description: Тип конфигурации групповой политики
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c0d3a0daa73fef30e5425e188958bdc54e61778d
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30164689"
---
# <a name="grouppolicyconfigurationtype-enum-type"></a><span data-ttu-id="dc6c1-103">тип перечисления Граупполициконфигуратионтипе</span><span class="sxs-lookup"><span data-stu-id="dc6c1-103">groupPolicyConfigurationType enum type</span></span>

> <span data-ttu-id="dc6c1-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dc6c1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dc6c1-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="dc6c1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dc6c1-106">Тип конфигурации групповой политики</span><span class="sxs-lookup"><span data-stu-id="dc6c1-106">Group Policy Configuration Type</span></span>

## <a name="members"></a><span data-ttu-id="dc6c1-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="dc6c1-107">Members</span></span>
|<span data-ttu-id="dc6c1-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="dc6c1-108">Member</span></span>|<span data-ttu-id="dc6c1-109">Значение</span><span class="sxs-lookup"><span data-stu-id="dc6c1-109">Value</span></span>|<span data-ttu-id="dc6c1-110">Описание</span><span class="sxs-lookup"><span data-stu-id="dc6c1-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dc6c1-111">policy</span><span class="sxs-lookup"><span data-stu-id="dc6c1-111">policy</span></span>|<span data-ttu-id="dc6c1-112">нуль</span><span class="sxs-lookup"><span data-stu-id="dc6c1-112">0</span></span>|<span data-ttu-id="dc6c1-113">Тип политики не является восстановленным значением, что означает, что значение удаляется, что позволяет использовать исходное значение конфигурации.</span><span class="sxs-lookup"><span data-stu-id="dc6c1-113">The policy type does not tattoo the value, which means the value is removed allowing the original configuration value to be used.</span></span> <span data-ttu-id="dc6c1-114">Тип политики заменяется параметром конфигурации приложения, поэтому приложение всегда знает значение.</span><span class="sxs-lookup"><span data-stu-id="dc6c1-114">The policy type supercedes application configuration setting so the application is always aware of the value.</span></span> <span data-ttu-id="dc6c1-115">Тип политики не позволяет пользователю изменять значение с помощью пользовательского интерфейса приложения.</span><span class="sxs-lookup"><span data-stu-id="dc6c1-115">The policy type prevents the user from modifying the value through the application's user interface.</span></span>|
|<span data-ttu-id="dc6c1-116">preference</span><span class="sxs-lookup"><span data-stu-id="dc6c1-116">preference</span></span>|<span data-ttu-id="dc6c1-117">1,1</span><span class="sxs-lookup"><span data-stu-id="dc6c1-117">1</span></span>|<span data-ttu-id="dc6c1-118">Тип предпочтения приводит к восстановлению значения, которое означает, что значение не удаляется из реестра.</span><span class="sxs-lookup"><span data-stu-id="dc6c1-118">The preference type does tattoo the value, which means the value is not removed from the registry.</span></span> <span data-ttu-id="dc6c1-119">Тип предпочтения перезапишет настраиваемое значение пользователем и не сохранит предыдущее значение.</span><span class="sxs-lookup"><span data-stu-id="dc6c1-119">The preference type will overwrite the user configured-value and does not retain the previous value.</span></span> <span data-ttu-id="dc6c1-120">Тип предпочтения не запрещает пользователю изменять значение с помощью пользовательского интерфейса приложения.</span><span class="sxs-lookup"><span data-stu-id="dc6c1-120">The preference type does not prevent the user from modifying the value through the application's user interface.</span></span>|




