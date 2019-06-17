---
title: тип перечисления Граупполициконфигуратионтипе
description: Тип конфигурации групповой политики
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4428493cc0a76fd22ee7155cacda22d38eb10204
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34975898"
---
# <a name="grouppolicyconfigurationtype-enum-type"></a><span data-ttu-id="3197a-103">тип перечисления Граупполициконфигуратионтипе</span><span class="sxs-lookup"><span data-stu-id="3197a-103">groupPolicyConfigurationType enum type</span></span>

> <span data-ttu-id="3197a-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3197a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3197a-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3197a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3197a-106">Тип конфигурации групповой политики</span><span class="sxs-lookup"><span data-stu-id="3197a-106">Group Policy Configuration Type</span></span>

## <a name="members"></a><span data-ttu-id="3197a-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="3197a-107">Members</span></span>
|<span data-ttu-id="3197a-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="3197a-108">Member</span></span>|<span data-ttu-id="3197a-109">Значение</span><span class="sxs-lookup"><span data-stu-id="3197a-109">Value</span></span>|<span data-ttu-id="3197a-110">Описание</span><span class="sxs-lookup"><span data-stu-id="3197a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3197a-111">policy</span><span class="sxs-lookup"><span data-stu-id="3197a-111">policy</span></span>|<span data-ttu-id="3197a-112">нуль</span><span class="sxs-lookup"><span data-stu-id="3197a-112">0</span></span>|<span data-ttu-id="3197a-113">Тип политики не является восстановленным значением, что означает, что значение удаляется, что позволяет использовать исходное значение конфигурации.</span><span class="sxs-lookup"><span data-stu-id="3197a-113">The policy type does not tattoo the value, which means the value is removed allowing the original configuration value to be used.</span></span> <span data-ttu-id="3197a-114">Тип политики заменяется параметром конфигурации приложения, поэтому приложение всегда знает значение.</span><span class="sxs-lookup"><span data-stu-id="3197a-114">The policy type supercedes application configuration setting so the application is always aware of the value.</span></span> <span data-ttu-id="3197a-115">Тип политики не позволяет пользователю изменять значение с помощью пользовательского интерфейса приложения.</span><span class="sxs-lookup"><span data-stu-id="3197a-115">The policy type prevents the user from modifying the value through the application's user interface.</span></span>|
|<span data-ttu-id="3197a-116">параметров</span><span class="sxs-lookup"><span data-stu-id="3197a-116">preference</span></span>|<span data-ttu-id="3197a-117">1,1</span><span class="sxs-lookup"><span data-stu-id="3197a-117">1</span></span>|<span data-ttu-id="3197a-118">Тип предпочтения приводит к восстановлению значения, которое означает, что значение не удаляется из реестра.</span><span class="sxs-lookup"><span data-stu-id="3197a-118">The preference type does tattoo the value, which means the value is not removed from the registry.</span></span> <span data-ttu-id="3197a-119">Тип предпочтения перезапишет настраиваемое значение пользователем и не сохранит предыдущее значение.</span><span class="sxs-lookup"><span data-stu-id="3197a-119">The preference type will overwrite the user configured-value and does not retain the previous value.</span></span> <span data-ttu-id="3197a-120">Тип предпочтения не запрещает пользователю изменять значение с помощью пользовательского интерфейса приложения.</span><span class="sxs-lookup"><span data-stu-id="3197a-120">The preference type does not prevent the user from modifying the value through the application's user interface.</span></span>|





