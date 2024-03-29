---
title: managedDevicePartnerReportedHealthState enum type
description: Доступные состояния здоровья для API здоровья устройств
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 78bd301c77f6437b1382dec4d845186879e5e117
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59040143"
---
# <a name="manageddevicepartnerreportedhealthstate-enum-type"></a>managedDevicePartnerReportedHealthState enum type

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Доступные состояния здоровья для API здоровья устройств

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|unknown|0|Состояние здоровья устройства пока не сообщается|
|активирована|1|Устройство было активировано мобильным партнером по защите от угроз, но пока не сообщается о состоянии здоровья.|
|отключено|2|Устройство было отключено мобильным партнером по защите от угроз. Состояние устройства неизвестно.|
|обеспечено|3|Устройство считается защищенным партнером по защите от мобильных угроз.|
|lowSeverity|4 |Устройство считается низкой угрозой со стороны партнера по защите от мобильных угроз.|
|mediumSeverity|5 |Устройство считается средней угрозой со стороны мобильного партнера по защите от угрозы.|
|highSeverity|6 |Устройство считается высокой угрозой со стороны партнера по защите от мобильных угроз.|
|unresponsive|7 |Устройство считается неосмотрительным партнером по защите от мобильных угроз. Состояние устройства неизвестно.|
|скомпрометирован|8 |Устройство считается скомпрометированным партнером по защите от угроз. Это означает, что устройство имеет активную угрозу или риск, которые не могут быть легко исправлены конечным пользователем, и пользователь должен связаться со своим ИТ-администратором.|
|неправильно сконфигурировали|9 |Устройство считается неправильным с партнером по защите от угроз. Это означает, что на устройстве отсутствует необходимый профиль или конфигурация для правильного функционирования партнера по защите от угроз и поэтому анализ угроз или рисков не может завершиться.|



