---
title: тип enum windowsPrivacyDataAccessLevel
description: Определение уровня доступа к определенной категории Windows конфиденциальности.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 5fa4ee09c3e931766fe3f76131841e0d69bdc65d
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58793847"
---
# <a name="windowsprivacydataaccesslevel-enum-type"></a>тип enum windowsPrivacyDataAccessLevel

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Определение уровня доступа к определенной категории Windows конфиденциальности.

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|notConfigured|0|Уровень доступа не указан, намерения не указаны. Устройство может вести себя как в UserInControl или ForceAllow. Это может зависеть от доступных данных конфиденциальности, Windows версий и других факторов.|
|forceAllow|1|Приложениям будет разрешен доступ к указанным данным конфиденциальности.|
|forceDeny|2|Приложениям будет отказано в доступе к указанным данным конфиденциальности.|
|userInControl|3|Пользователям будет предложено, когда приложения попытаются получить доступ к указанным данным конфиденциальности.|



