---
title: тип перечисления Фиреваллпрешаредкэйенкодингмесодтипе
description: Возможные значения для Фиреваллпрешаредкэйенкодингмесод
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 36c49a0c97ac8f2e9267f20762fd6e748d952240
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31786163"
---
# <a name="firewallpresharedkeyencodingmethodtype-enum-type"></a><span data-ttu-id="f626b-103">тип перечисления Фиреваллпрешаредкэйенкодингмесодтипе</span><span class="sxs-lookup"><span data-stu-id="f626b-103">firewallPreSharedKeyEncodingMethodType enum type</span></span>

> <span data-ttu-id="f626b-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f626b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f626b-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f626b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f626b-106">Возможные значения для Фиреваллпрешаредкэйенкодингмесод</span><span class="sxs-lookup"><span data-stu-id="f626b-106">Possible values for firewallPreSharedKeyEncodingMethod</span></span>

## <a name="members"></a><span data-ttu-id="f626b-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="f626b-107">Members</span></span>
|<span data-ttu-id="f626b-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="f626b-108">Member</span></span>|<span data-ttu-id="f626b-109">Значение</span><span class="sxs-lookup"><span data-stu-id="f626b-109">Value</span></span>|<span data-ttu-id="f626b-110">Описание</span><span class="sxs-lookup"><span data-stu-id="f626b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f626b-111">Девицедефаулт</span><span class="sxs-lookup"><span data-stu-id="f626b-111">deviceDefault</span></span>|<span data-ttu-id="f626b-112">нуль</span><span class="sxs-lookup"><span data-stu-id="f626b-112">0</span></span>|<span data-ttu-id="f626b-113">Значение не настроено Intune, не переопределять значение устройства по умолчанию, настроенное пользователем</span><span class="sxs-lookup"><span data-stu-id="f626b-113">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="f626b-114">нет</span><span class="sxs-lookup"><span data-stu-id="f626b-114">none</span></span>|<span data-ttu-id="f626b-115">1,1</span><span class="sxs-lookup"><span data-stu-id="f626b-115">1</span></span>|<span data-ttu-id="f626b-116">Общий ключ не кодируется.</span><span class="sxs-lookup"><span data-stu-id="f626b-116">Preshared key is not encoded.</span></span> <span data-ttu-id="f626b-117">Вместо этого он хранится в расширенном формате символов</span><span class="sxs-lookup"><span data-stu-id="f626b-117">Instead, it is kept in its wide-character format</span></span>|
|<span data-ttu-id="f626b-118">utF8</span><span class="sxs-lookup"><span data-stu-id="f626b-118">utF8</span></span>|<span data-ttu-id="f626b-119">2</span><span class="sxs-lookup"><span data-stu-id="f626b-119">2</span></span>|<span data-ttu-id="f626b-120">Кодирование общего ключа с помощью UTF – 8</span><span class="sxs-lookup"><span data-stu-id="f626b-120">Encode the preshared key using UTF-8</span></span>|





