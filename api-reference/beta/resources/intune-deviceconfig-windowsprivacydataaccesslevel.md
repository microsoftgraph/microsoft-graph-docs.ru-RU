---
title: тип enum windowsPrivacyDataAccessLevel
description: Определение уровня доступа к определенной категории Windows конфиденциальности.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: c45d78e06ac44fc30cb631359f213a90d8ba8f6a
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59105897"
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



