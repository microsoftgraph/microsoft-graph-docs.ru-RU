---
title: тип перечисления Фиреваллпрешаредкэйенкодингмесодтипе
description: Возможные значения для Фиреваллпрешаредкэйенкодингмесод
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 68afa14e7bee7fec1e91af002c23d81b526d573f
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42791746"
---
# <a name="firewallpresharedkeyencodingmethodtype-enum-type"></a><span data-ttu-id="a3b1e-103">тип перечисления Фиреваллпрешаредкэйенкодингмесодтипе</span><span class="sxs-lookup"><span data-stu-id="a3b1e-103">firewallPreSharedKeyEncodingMethodType enum type</span></span>

> <span data-ttu-id="a3b1e-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a3b1e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a3b1e-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a3b1e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a3b1e-106">Возможные значения для Фиреваллпрешаредкэйенкодингмесод</span><span class="sxs-lookup"><span data-stu-id="a3b1e-106">Possible values for firewallPreSharedKeyEncodingMethod</span></span>

## <a name="members"></a><span data-ttu-id="a3b1e-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="a3b1e-107">Members</span></span>
|<span data-ttu-id="a3b1e-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="a3b1e-108">Member</span></span>|<span data-ttu-id="a3b1e-109">Значение</span><span class="sxs-lookup"><span data-stu-id="a3b1e-109">Value</span></span>|<span data-ttu-id="a3b1e-110">Описание</span><span class="sxs-lookup"><span data-stu-id="a3b1e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a3b1e-111">девицедефаулт</span><span class="sxs-lookup"><span data-stu-id="a3b1e-111">deviceDefault</span></span>|<span data-ttu-id="a3b1e-112">нуль</span><span class="sxs-lookup"><span data-stu-id="a3b1e-112">0</span></span>|<span data-ttu-id="a3b1e-113">Значение не настроено Intune, не переопределять значение устройства по умолчанию, настроенное пользователем</span><span class="sxs-lookup"><span data-stu-id="a3b1e-113">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="a3b1e-114">none</span><span class="sxs-lookup"><span data-stu-id="a3b1e-114">none</span></span>|<span data-ttu-id="a3b1e-115">1,1</span><span class="sxs-lookup"><span data-stu-id="a3b1e-115">1</span></span>|<span data-ttu-id="a3b1e-116">Общий ключ не кодируется.</span><span class="sxs-lookup"><span data-stu-id="a3b1e-116">Preshared key is not encoded.</span></span> <span data-ttu-id="a3b1e-117">Вместо этого он хранится в расширенном формате символов</span><span class="sxs-lookup"><span data-stu-id="a3b1e-117">Instead, it is kept in its wide-character format</span></span>|
|<span data-ttu-id="a3b1e-118">utF8</span><span class="sxs-lookup"><span data-stu-id="a3b1e-118">utF8</span></span>|<span data-ttu-id="a3b1e-119">2</span><span class="sxs-lookup"><span data-stu-id="a3b1e-119">2</span></span>|<span data-ttu-id="a3b1e-120">Кодирование общего ключа с помощью UTF – 8</span><span class="sxs-lookup"><span data-stu-id="a3b1e-120">Encode the preshared key using UTF-8</span></span>|



